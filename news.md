---
title: Latest News
layout: single
excerpt: All the latest Charnwood Eco Hub updates
header:
  overlay_image: /assets/img/charnwood-eco-hub-banner.jpg
---

{% raw %}
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>
{% endraw %}
