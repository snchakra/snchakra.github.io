---
layout: page
title:  "Sleepy Head"
permalink: /sleepy-head/
---
I couldn’t resist.  
Every time you fall asleep, it’s like the world pauses for just you.  
I saved a few of those little moments here — just for me to remember, just for me to smile.  

<div class="gallery">
  {% for i in (1..7) %}
    <div class="gallery-item">
      <img src="{{ '/images/sleepy/image' | append: i | append: '.jpg' | relative_url }}" alt="Gallery image {{ i }}">
    </div>
  {% endfor %}
</div>

  <!-- Add the video -->
  <div class="gallery-item">
    <video controls>
      <source src="{{ '/images/sleepy/image8.mp4' | relative_url }}" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>


<style>
.gallery {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 20px;
  justify-items: center;
  margin-top: 25px;
}
.gallery-item {
  text-align: center;
}
.gallery-item img, .gallery-item video {
  width: 100%;
  max-width: 350px;
  height: auto;
  border-radius: 14px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.2);
  transition: transform 0.25s ease, box-shadow 0.25s ease;
}
.gallery-item img:hover, .gallery-item video:hover {
  transform: scale(1.03);
  box-shadow: 0 8px 20px rgba(0,0,0,0.25);
}
.caption {
  font-size: 1em;
  margin-top: 8px;
  color: #555;
  font-style: italic;
  line-height: 1.3;
}
@media (max-width: 600px) {
  .gallery {
    grid-template-columns: 1fr;
    gap: 15px;
  }
  .gallery-item img, .gallery-item video {
    max-width: 90%;
  }
}
</style>