---
layout: page
title: Pagina de inicio
permalink: /
description: Descripcion de la pagina de inicio
---

<div class="row">
  {% for post in site.posts %}
    <div class="col-sm-4">
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
      {{ post.excerpt }}
    </div>
  {% endfor %}
</div>