---
layout: page
title: Photos
permalink: /photos/
sub-title: Photos
---
<div class="photo-content">
  {% assign image_files = site.static_files | where: "image", true %}
  {% for myimage in image_files %}
    <img class="gallery" src="{{ myimage.path }}" alt="">
  {% endfor %}
</div>
