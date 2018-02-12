---
layout: default
permalink: /all/
---

<div class="home">

  <h1 class="post-title">文章</h1>



  <ul class="post-list">
  {% for post in site.posts %}
      <li>
        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
          <span class="post-meta"><small>{{ post.date | date: "%b %-d, %Y" }}</small></span>
        </h2>
         
      </li>
    {% endfor %}
  </ul>
  


{% include pagination.html %}