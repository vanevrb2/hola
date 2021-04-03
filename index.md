---
layout: default
---

<form class="search" action="/search">
    <input type="text" placeholder="Search" name="q" value="{{ search.terms | escape }}"  />
    <input type="submit" value="Search" />
</form>

<div class="row">
  {% for post in site.posts %}
    <div class="col-sm-12">
    <div class="card">
      <div class="card-body">
        <h5 class="card-title"><h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1></h5>
        <p class="card-text"> {{ post.excerpt }}</p>
                <a href="{{ site.baseurl }}{{ post.url }}" class="btn btn-primary">Read More</a>

      </div>
    </div>
  </div>
  {% endfor %}
</div>
