---
title: Music
permalink: "/music/"
layout: page
---

{% for album in site.music reversed %}
<h2>{{ album.title }}</h2>
<span class="music-type">{{ album.type }}</span>
<div class="row">
  <div class="grid-half">
    <a href="{{ album.link }}">
      <img
        class="hover-askew"
        src="{{ album.image_path }}"
        alt="{{ album.title }}"
        width="320"
        height="320"
    /></a>
    <p>
      <a href="{{ album.link }}" class="more"
        >Purchase/Stream on Bandcamp&rarr;</a
      >
    </p>
  </div>
  <div class="grid-half">{{ album.content }}</div>
</div>
<hr />
{% endfor %}

<p>
  Our complete discography is available on our
  <a href="https://theordinarythings.bandcamp.com/music">bandcamp music page</a
  >.
</p>
