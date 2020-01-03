---

title: PDF Archive Files
layout: col-sidebar

---

<ul>
{% for item in site.static_files %}
{% assign fpath = item.path | lower %}
{% if fpath contains '.pdf' %}
<li><a href='{{item.url}}'>{{item.name}}</a></li>
{% endif %}
{% endfor %}
</ul>
