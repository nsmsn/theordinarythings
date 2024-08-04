---
title: Music
permalink: "/music/"
layout: page
---

<h2>IV</h2>
<span class="music-type">Album</span>
<div class="row">
  <div class="grid-half">
    <a href="https://music.apple.com/us/album/iv/1759902825">
      <img
        class="hover-askew"
        src="https://d2w9rnfcy7mm78.cloudfront.net/29790651/original_53b0b83161ee0c228c356b56d8d9840f.jpg?1722730956?bc=0"
        alt="Four"
        width="320"
        height="320"
    /></a>
    <p>
      <a href="https://music.apple.com/us/album/iv/1759902825" class="more"
        >Apple Music &rarr;</a
      ></br>
      <a href="https://open.spotify.com/album/41KH3qwfnbo7RDEaPNuWvN?si=ao6_7ULJQIKP6QXWwbul0Q" class="more"
        >Spotify &rarr;</a
      ></br>
    </p>
  </div>
  <div class="grid-half">
1. Illuminate
2. Live in Love
3. Heaven 1
4. Take My Life
5. Heaven 2
6. It's Time
7. Heaven 3
8. Lost My Life
9. Hear
10. 1,000 Years
11. Shadows Fall

Released August 1, 2024

Music and Lyrics by The Ordinary Things
</div>
</div>
<hr />

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
        >Purchase/Stream &rarr;</a
      >
    </p>
  </div>
  <div class="grid-half">{{ album.content }}</div>
</div>
<hr />
{% endfor %}

<p>
  Our complete discography is available on <a href="https://music.apple.com/us/artist/the-ordinary-things/1479755190">Apple Music</a>, <a href="https://open.spotify.com/artist/6OPNOPE1FtWA1dG7CwLPmz?si=N2bQxWjfStS3f8-fiOcutQ">Spotify</a>, and
  <a href="https://theordinarythings.bandcamp.com/music">Bandcamp</a
  >.
</p>
