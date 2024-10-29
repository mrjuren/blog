---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: "最新動態"
pagination:
  enabled: true
  per_page: 5
---
<link rel="stylesheet" href="{{ '/assets/css/main.css' | relative_url }}">
<div class="latest-updates">
  {% for post in paginator.posts %}
    <div class="post-preview">
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <p class="tags">
        {% for tag in post.tags %}
          <span class="tag">{{ tag }}</span>
        {% endfor %}
      </p>
      <p class="excerpt">{{ post.excerpt | truncatewords: 25 }}</p>
      <p><a href="{{ post.url }}">顯示更多</a></p>
    </div>
  {% endfor %}

  <div class="pagination">
    {% if paginator.previous_page %}
      <a href="{{ paginator.previous_page_path }}">上一頁</a>
    {% endif %}
    {% if paginator.next_page %}
      <a href="{{ paginator.next_page_path }}">下一頁</a>
    {% endif %}
  </div>
</div>
