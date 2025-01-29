aliases: 
  - {{title | replace(":", "") | replace("#", "") | replace("^", "") | replace("|", "") | replace("\[", "") | replace("\]", "") | replace("\\", "") | replace("/", "")}}
  - {{citekey}}
<%"---"%>
<%*
    let citekey = "{{citekey}}"; 
    let date = tp.date.now("YYYY-MM-DD");
    await tp.file.rename(`${citekey}_ZoteroA`);
%>



# Commented Annotations
{% for annotation in annotations %}
  {%- if annotation.hashTags and annotation.comment -%}
- {{ annotation.comment ~ ' ' ~ annotation.hashTags}}
{%endif-%}
{%endfor%}

---
# Categorical Annotations

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
{%- if annotation.colorCategory | lower == color and annotation.annotatedText -%}
	- <mark class="hltr-{{annotation.colorCategory | lower}}">"{{  annotation.annotatedText | escape}}"</mark> [Page {{annotation.page}}](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.page}}&annotation={{annotation.id}})
{%endif %}
{%- if (annotation.colorCategory | lower == color and annotation.comment) and not annotations.hashTags %}
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

### Current Annotation
	```dataview
	table item.text as "Related Annotation"
	FROM "Paper Analysis"
	FLATTEN file.lists as item
	WHERE contains(item.tags, "#concepts")
	```

### All Annotations
	```dataview
	table WITHOUT ID item.text as "Related Annotation"
	FROM "Paper Analysis"
	FLATTEN file.lists as item
	WHERE contains(item.tags, "#concepts")
	WHERE file.path = this.file.path
	```
	
	
