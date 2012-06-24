---
layout: default
---
<div>
{% for post in site.posts limit: 5 %}
<article>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p class="meta">
        <span class="time">
          <time datetime="{{ post.date | date:"%Y-%m-%d" }}">{{ post.date | date:"%Y-%m-%d" }}</time>
        </span>
        {% if post.tags %}
        <span class="tags">
          {% for tag in post.tags %}
          <a href="/tags.html#{{ tag }}" title="{{ tag }}">#{{ tag }}</a>
          {% endfor %}
        </span>
        {% endif %}
    </p>
    <p class="post">
        {{ post.content }}
    </p>
</article>
{% endfor %}
</div>
<div class="center">
    <a href="/archive.html" class="circle-wrapper">
    <div class="circle">&nbsp;</div>
    <div class="circle">&nbsp;</div>
    <div class="circle">&nbsp;</div>
    </a>
</div>