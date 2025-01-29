<%"---"%>
aliases: 
  - {{title | replace(":", "") | replace("#", "") | replace("^", "") | replace("|", "") | replace("\[", "") | replace("\]", "") | replace("\\", "") | replace("/", "")}}
  - {{citekey}}
<%"---"%>
<%*
    let citekey = "{{citekey}}"; 
    let date = tp.date.now("YYYY-MM-DD");
    await tp.file.rename(`${citekey}_Analysis`);
%>


{% set color_labels = {
    'red': 'Definitions',
    'orange': 'Applications',
    'yellow': 'Technical Details',
    'green': 'Conceptual',
    'blue': 'Personal Insights',
    'purple': 'Literary Note To Lookup Later'
} %}



{%- for color, label in color_labels -%}
##  <h1 class="color-{{ color }}">{{ label }}</h>
{% for annotation in annotations %}
{%- if annotation.colorCategory | lower == color and annotation.annotatedText and not annotation.hashTags -%}
	- "<mark class="hltr-{{annotation.colorCategory | lower}}">"{{  annotation.annotatedText | escape}}"</mark>" [Page {{annotation.page}}](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.page}}&annotation={{annotation.id}})
{%endif %}
{%- if annotation.colorCategory | lower == color and annotation.annotatedText and annotation.hashTags -%}
{%- set textInsert = annotation.annotatedText ~ ' ' ~ annotation.hashTags -%}
	- <mark class="hltr-{{annotation.colorCategory | lower}}">"{{  annotation.annotatedText | escape}}"</mark>  [Page {{annotation.page}}](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.page}}&annotation={{annotation.id}}) {{annotation.hashTags}}
{%endif %}
{%- if (annotation.colorCategory | lower == color and annotation.comment) and not annotation.hashTags %}
	- {{annotation.comment}} 
{%endif %} 
{%- if annotation.colorCategory | lower == color and annotation.comment and annotation.hashTags%}
	- {{ annotation.comment ~ ' ' ~ annotation.hashTags}}
{%endif %} 
{%- if annotation.colorCategory | lower == color and annotation.imageRelativePath -%}
	![[{{annotation.imageRelativePath}}]]
{%endif %} 
{%-endfor%}
{%endfor %}

---
# 🧠 Key Ideas
- 
---
# ⚙️ Project Relations
- 
---
# 📄 Related Literature 
- 
---
# 🏷️ Tags

# Unique tag Groups 
{%  set tag_dict = []%}
{%-  for annotation in annotations -%}
{%- if annotation.hashTags -%}
{%- set cur_var = annotation.hashTags -%}
{%- set _  = tag_dict.push(cur_var) -%}
{%-endif-%}
{%-endfor-%}


{%- set uniqueValues = [] -%}
{%- for item in tag_dict -%}
    {%- if item not in uniqueValues -%}
        {%- set _ = uniqueValues.push(item) -%}
    {%- endif -%}
{%- endfor -%}

{%- for tag in uniqueValues %}
{{tag}}
{%-endfor%}


# 🏷️ Tags Groups within Current Paper



{%- for tag in uniqueValues %}
# {{tag}}

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "{{tag}}", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "{{tag}}")
WHERE file.path = this.file.path
```

{%endfor%}

---

# 🏷️ Tags Groups within All Papers

{%- for tag in uniqueValues %}
# {{tag}}

```dataview
table WITHOUT ID file.link as "Paper",
replace(item.text, "{{tag}}", "")  as "Related Annotations"
FROM "Paper Analysis"
FLATTEN file.lists as item
WHERE econtains(item.text, "{{tag}}")
```

{%endfor%}


