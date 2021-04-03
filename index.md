---
layout: default
---

<div class="posts">
  {% for post in site.sliders %}
      <img src="{{ site.baseurl }}{{ post.url }}" />
  {% endfor %}
</div>
