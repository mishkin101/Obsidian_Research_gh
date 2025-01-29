<%"---"%>
tags: 📥️/📜️/🟥️
publish: true
aliases: 
  - {{title | replace(":", "") | replace("#", "") | replace("^", "") | replace("|", "") | replace("\[", "") | replace("\]", "") | replace("\\", "") | replace("/", "")}}
  - {{citekey}}
<%"---"%>
<%*
	let title = "{{title | replace(':', '') | replace('#', '') | replace('^', '') | replace('|', '') | replace('\[', '') | replace('\]', '') | replace('\\', '') | replace('/', '')}}";
	let date = tp.date.now("YYYY-MM-DD");
	await tp.file.rename(`& ${date} ${title}`);
_%>

> [!link]
> zotero_link:: {{pdfZoteroLink}}

> [!cite]
> citekey:: {{citekey}}

> [!abstract]
> abstract:: {{abstractNote}}

> [!keywords]
> keywords:: {{allTags}}

> [!authors]
> authors:: {{authors}}{{directors}}

> [!meta]
> url:: {{url}}
> doi:: {{doi}}

> [!related]
{% for relation in relations -%}
{%- if relation.citekey -%}
> related:: {{relation.citekey}}
{% endif -%}
{%- endfor %}

```dataview
TABLE created, updated as modified, tags, type
FROM ""
WHERE related != null
AND contains(related, "{{citekey}}")
```

> [!hypothesis]
> hypothesis:: 

> [!methodology] 
> methodology:: 

> [!result] Result(s) 
> results::

> [!summary] Summary of Key Points
> summary:: 

## Notes

| <mark class="hltr-grey">Highlight Color</mark> | Meaning                       |
| ---------------------------------------------- | ----------------------------- |
| <mark class="hltr-red">Red</mark>              | Definitions                   |
| <mark class="hltr-orange">Orange</mark>        | Applications                  |
| <mark class="hltr-yellow">Yellow</mark>        | Technical Details             |
| <mark class="hltr-green">Green</mark>          | Conceptual                    |
| <mark class="hltr-blue">Blue</mark>            | Personal Insights             |
| <mark class="hltr-purple">Purple</mark>        | Literary Note To Lookup Later |

{% for annotation in annotations -%}
    {%- if annotation.annotatedText -%} 
		- <mark class="hltr-{{annotation.colorCategory | lower}}">"{{annotation.annotatedText | escape}}”</mark> [Page {{annotation.page}}](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.page}}&annotation={{annotation.id}})
    {%- endif %} 
    {%- if annotation.imageRelativePath -%}
    ![[{{annotation.imageRelativePath}}]] {%- endif %} 
{%- if annotation.comment %} 
	- {{annotation.comment}} 
{%-endif %} 
{% endfor %}








> [!context]
> ==(How this article relates to other work in the field; how it ties in with key issues and findings by others, including yourself)==
> context:: 

> [!significance]
> ==(to the field; in relation to your own work)==
> significance:: 
