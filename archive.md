---
layout: page
title: Archive
---

## Blog Posts

<div id="archive">
	{% for post in site.posts %}
    <div class="card">
      
      <a href="{{ post.url }}" class="heading">Blog #{{ post.number }}: {{ post.title }}<br/></a>

      <p class="tag">
        <i class="fa fa-tags fa-flip-horizontal"></i> 
        {% if post.tags %}
        {% for tag in post.tags %}
        <a href="{{site.baseurl}}/tag/{{ tag }}">{{ tag }}</a>
        {% endfor %}
        {% endif %}
      </p>
    </div>
  {% endfor %}
</div>