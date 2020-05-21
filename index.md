---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---
{% for page in site.pages %}
{% if page.layout == 'list' %}
<a href="{{ site.url }}{{ page.url }}">{{ page.path | split: "." | first}}</a>
<hr />
{% endif %}
{% endfor %}