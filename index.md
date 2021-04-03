---
layout: default
---

<form class="search" action="/search">
    <input type="text" placeholder="Search" name="q" value="{{ search.terms | escape }}"  />
    <input type="submit" value="Search" />
</form>
<div class="posts">
  {% for post in site.posts %}
    <article class="post">

      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>

      <div class="entry">
        {{ post.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>
  {% endfor %}
</div>
