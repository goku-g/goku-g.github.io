---
layout: page
title: Gallery
permalink: /gallery/
gallery_images:
  - file: robot-test.jpg
    caption: "Field testing the path planning algorithm"
  - file: lab-setup.jpg
    caption: "Our Jetson Nano setup"
  - file: wheat-crops.jpg
    caption: "Data collection in the wheat field"
---

<div class="row">
{% for item in page.gallery_images %}
  <div class="col-sm-6 col-md-4 mb-4">
    <div class="card h-100">
      <img src="{{ site.baseurl }}/assets/images/gallery/{{ item.file }}" class="card-img-top" alt="{{ item.caption }}">
      <div class="card-body">
        <p class="card-text text-center text-muted">{{ item.caption }}</p>
      </div>
    </div>
  </div>
{% endfor %}
</div>