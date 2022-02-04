---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

<!-- {% if site.tags!="" %}
   {%include collecttags.html%}
{%endif%} -->

<body>
{% for row in site.data.data %}
  <div>
    "{{row.Object}}"
  </div>
{% endfor %}
</body>
