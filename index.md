---
layout: default
---

<div class="posts">
  {% for slider in site.sliders %}
      <img src="{{ site.baseurl }}{{ slider.url }}.png" />
  {{ site.baseurl }}{{ slider.url }}
  {% endfor %}
</div>
