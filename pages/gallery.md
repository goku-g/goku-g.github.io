---
layout: events
title: Gallery
subtitle: null
banner_image: /assets/images/vintage-newspaper-print-downsize.jpg
permalink: /gallery/

gallery_images:
  - file: robot-test.jpg
    caption: "Field testing the path planning algorithm"
    href: /newsfeed/dec10-2025/ # link if this associated with any events (eg. /newsfeed/dec10-2025/)
  - file: lab-setup.jpg
    caption: "Our Jetson Nano setup"
    href: null # link if this associated with any events (eg. /newsfeed/dec10-2025/)
  - file: wheat-crops.png
    caption: "Data collection in the wheat field"
    href: /newsfeed/feb10-2025/ # link if this associated with any events (eg. /newsfeed/dec10-2025/)
  - file: wheat-crops.png
    caption: "Data collection in the wheat field"
    href: /newsfeed/feb10-2025/ # link if this associated with any events (eg. /newsfeed/dec10-2025/)
  - file: wheat-crops.png
    caption: "Data collection in the wheat field"
    href: /newsfeed/feb10-2025/ # link if this associated with any events (eg. /newsfeed/dec10-2025/)
  - file: wheat-crops.png
    caption: "Data collection in the wheat field"
    href: /newsfeed/feb10-2025/ # link if this associated with any events (eg. /newsfeed/dec10-2025/)
  - file: wheat-crops.png
    caption: "Data collection in the wheat field"
    href: /newsfeed/feb10-2025/ # link if this associated with any events (eg. /newsfeed/dec10-2025/)
---

<!-- Content here would show up in body -->
<div class="row">
{% for item in page.gallery_images %}
  <div class="col-sm-6 col-md-4 mb-4">
    <div class="card h-100 mb-0">
      <!-- <img src="{{ site.baseurl }}/assets/images/gallery/{{ item.file }}" class="card-img" alt="{{ item.caption }}"> -->
      <!-- if any image has the href beside the caption then add anchor tag for href -->
      {% if item.href != nil %}
      <a href="{{item.href}}">
      {% endif %}
      <img src="{{ site.baseurl }}/assets/images/gallery/{{ item.file }}" 
           class="card-img" 
           alt="{{ item.caption }}"
           style="height: 250px; object-fit: contain; width: 100%; background-color: #f8f9fa;">
      {% if item.href != nil %}
      </a>
      {% endif %}
      <div class="card-body-bottom p-3">
        <p class="card-text text-center text-muted m-0 small">{{ item.caption }}</p>
      </div>
    </div>
  </div>
{% endfor %}
</div>
