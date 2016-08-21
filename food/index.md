---
layout: default
title: food
---
<ul class="posts">
{% for post in site.posts %}
  {% if post.category == 'food' %}
  <li data-post="scroll-in-view" class="post {{post.category}}">
    <a href="{{ post.url }}">
	  	<img src="{{post.image}}" />
	  </a>
  </li>
  {% endif %}
{% endfor %}
</ul>