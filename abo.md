---
layout: page
title: abo
permalink: /abo/
---


<div id="carouselExampleControls" class="carousel slide" data-bs-ride="carousel">
  <div class="carousel-inner ">
    
{% assign image_files = site.static_files | where: "image", true %}
{% for myImage in image_files %}
    <div class="carousel-item {% if myImage.path == "/assets/img/sliders/1.png" %}active{% endif %}">
      <img src="{{ site.baseurl }}{{ myImage.path }}"  class="d-block w-100" alt="...">
    </div>
    {% endfor  %}

    
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>
