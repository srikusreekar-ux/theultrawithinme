---
layout: default
title: Gallery
---

# Photo Gallery

<div class="gallery-grid">
  {% for img in site.static_files %}
    {% if img.path contains '/assets/images/gallery/' %}
      <figure>
        <img src="{{ img.path }}" alt="{{ img.name }}" />
      </figure>
    {% endif %}
  {% endfor %}
</div>
