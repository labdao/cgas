## {{title}}
{{citekey}}
#paper #source #cgas 

### Formatted Bibliography
{{bibliography}}

{% if abstractNote %}
### Abstract
{{abstractNote}}
{% endif %}

{%- for attachment in attachments | filterby("path", "endswith", ".pdf") %}  
[[{{attachment.title}}]]
{%- endfor -%}.

### Annotations
{%- macro calloutHeader(type, color) -%}  
{%- if type == "highlight" -%}  
<mark style="background-color: {{color}}">Highlight</mark>  
{%- endif -%}{%- if type == "text" -%}  
Note  
{%- endif -%}  
{%- endmacro -%}{%- set annots = annotations | filterby("date", "dateafter", lastExportDate) -%}  
{%- if annots.length > 0 %}  
Exported: {{exportDate | format("YYYY-MM-DD h:mm a")}}
{% for annot in annots -%}  
> {{calloutHeader(annot.type, annot.color)}}  
{%- if annot.annotatedText %}  
> {{annot.annotatedText | nl2br}}  
{%- endif -%}  
{%- if annot.imageRelativePath %}  
> ![[{{annot.imageRelativePath}}]]  
{%- endif %}  
> [page {{annot.page}}](file://{{annot.attachment.path | replace(" ", "%20")}}) 
  {{annot.date | format("YYYY-MM-DD#h:mm a")}} 
{%- if annot.comment %}  
> - {{annot.comment | nl2br}}  
{% endif %}
{% endfor -%}  
{% endif -%}
