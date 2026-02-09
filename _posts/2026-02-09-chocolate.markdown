---
layout: protected-post
title: "Chocolate Day 🍫"
date:   2026-02-09
categories: jekyll update
password: h2o
riddle: “I flow, I splash, I make waves, yet my name is just three characters long Guess me and our first binge awaits.”
---

<p style="text-align:center;font-style:italic;">
Measure my love in dust,<br>
the layers on photographs of the summer,<br>
the ones that we spent together.<br><br>

Measure it in the dust atop my insecurities<br>
and your wounds that you thought would never heal<br><br>

Measure my love in the dust<br>
thats mixed in the ash of things<br>
I burned down to get to you,<br>
both around and inside my body,<br>
when my body is nothing but dust.<br>
Dust of the millions of stars that died,<br>
to create the life we are in.<br><br>

Measure my love in that--<br>
in the magic,<br>
in the monument of color<br>
that springs from the earth,<br>
or a red song of devotion,<br>
a word that frames but cannot contain its limitlessness.
</p>

<div class="gallery">
  {% for i in (1..7) %}
    <div class="gallery-item">
      <img src="{{ '/images/chocolate/image' | append: i | append: '.JPG' | relative_url }}" alt="Gallery image {{ i }}">
    </div>
  {% endfor %}
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
.gallery-item img {
  width: 100%;
  max-width: 350px;
  height: auto;
  border-radius: 14px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.2);
  transition: transform 0.25s ease, box-shadow 0.25s ease;
}
.gallery-item img:hover {
  transform: scale(1.05);
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
  .gallery-item img {
    max-width: 90%;
  }
}
</style>