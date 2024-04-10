---
title: Charnwood Eco Hub
layout: single
excerpt: Helping Charnwood to reduce its carbon footprint
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
