---
layout: page
title: Will Vokins
tagline: Network Security and Cryptography
---
{% include JB/setup %}

Hello, welcome to my GitHub.  I am a full-time web developer living in Bristol, England.  I enjoy researching web security and crpytography in my spare time and use this website to share my research with the world.  I hope what you find interests you as it has interested me.

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>