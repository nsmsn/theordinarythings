---
title: About
permalink: "/about/"
layout: page
---

<p>
  The Ordinary Things formed in Albuquerque in 2018.
</p>

<p>&nbsp;</p>

{% for bio in site.bios %}
<div class="row">
  <div class="grid-fourth">
    <img
      src="{{ bio.image_path }}"
      alt="{{ bio.name }}"
      width="160"
      height="160"
    />
  </div>
  <div class="grid-three-fourths">
    <h2>
      {{ bio.name }}<br />
      <span class="bio-role">{{ bio.role }}</span>
    </h2>
    <p>{{ bio.content }}</p>
    <p>&nbsp;</p>
  </div>
</div>

{% endfor %}
