---
layout: default
---

{% assign image_files = site.static_files | where: "image", true %}
{% for myImage in image_files %}
<img src="{{ site.baseurl }}{{ myImage.path }}">
{% endfor  %}
