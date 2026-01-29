---
layout: events
title: Gallery
subtitle: null
banner_image: null
permalink: /gallery/

gallery_images:
  - file: robot-test.jpg
    caption: "Field testing the path planning algorithm"
  - file: lab-setup.jpg
    caption: "Our Jetson Nano setup"
  - file: wheat-crops.png
    caption: "Data collection in the wheat field"
---

<!-- Content here would show up above your list of -->
<div class="row">
{% for item in page.gallery_images %}
  <div class="col-sm-6 col-md-4 mb-4">
    <div class="card h-100 mb-0">
      <!-- <img src="{{ site.baseurl }}/assets/images/gallery/{{ item.file }}" class="card-img" alt="{{ item.caption }}"> -->
      <img src="{{ site.baseurl }}/assets/images/gallery/{{ item.file }}" 
           class="card-img" 
           alt="{{ item.caption }}"
           style="height: 250px; object-fit: contain; width: 100%; background-color: #f8f9fa;">
      
      <div class="card-body-bottom p-3">
        <p class="card-text text-center text-muted m-0 small">{{ item.caption }}</p>
      </div>
      
    </div>
  </div>
{% endfor %}
</div>
