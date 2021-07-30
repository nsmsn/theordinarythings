---
title: "Video"
permalink: "/video/"
layout: page
---

{% for video in site.video reversed %}
<h2>{{ video.title }}</h2>
<div class="embed-container">
  <iframe src="{{ video.link }}" frameborder="0" allowfullscreen></iframe>
</div>
<p>{{ video.content }}</p>
<hr />
{% endfor %}

<p>
  Subscribe to our
  <a href="https://www.youtube.com/channel/UCLIVmEj9o8LI3zCdQ8S3c6Q"
    >YouTube channel</a
  >
  to see our latest videos when they premiere.
</p>
