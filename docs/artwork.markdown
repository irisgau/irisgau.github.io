---
layout: page
title: Artwork
permalink: /artwork/
---

# Digital

{% include image-gallery.html folder="/assets/images/artwork/digital" %}
<div class="gallery">

  {% for file in site.static_files %}
    {% if file.path contains '/assets/images/artwork/digital' and file.extname == '.jpeg'%}
      <img src="{{ file.path }}" alt="Gallery Image" height=200>
    {% endif %}
  {% endfor %}
</div>

# Paint
<div class="gallery">
  {% for file in site.static_files %}
    {% if file.path contains '/assets/images/artwork/paint' and file.extname == '.jpeg'%}
      <img src="{{ file.path }}" alt="Gallery Image" height=200>
    {% endif %}
  {% endfor %}
</div>


# Pencil
<div class="gallery">
  {% for file in site.static_files %}
    {% if file.path contains '/assets/images/artwork/pencil' and file.extname == '.jpeg'%}
      <img src="{{ file.path }}" alt="Gallery Image" height=200>
    {% endif %}
  {% endfor %}
</div>
