---
title: "About"
mytitle: "About Team ARAM"
layout: splash
permalink: /about/
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/about.jpg
excerpt: "Animation, Robotics, and Machine Learning"
---

## Who We Are

Team ARAM is a cross-institutional research group focusing on **A**nimation, **R**obotics, **A**nd **M**achine Learning, led by [Nam Hee Gordon Kim](https://namheegordonkim.github.io). Team ARAM is a platform for peer-to-peer collaboration aiming for cutting edge research in embodied intelligence.

## People

### --- Aalto University ---

<style>
  a {
  text-decoration: none;
}

a:hover {
  /* color: white; */
  text-decoration: underline;
  cursor: pointer;
}

div.people {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}

div.person {
  width: 412px;  
}

p.person {
  text-align: center;
  margin: 5px 0;
}

img.person {
  object-fit:cover;
  width:80%;
  aspect-ratio: 1/1;
  border-radius:50%;
}
</style>

<div class="people">
  {% for person in site.data.people.aalto %}
    {% if person.headshot == ""%}
    {% assign headshot = "/assets/imgs/gigachad.jpg" %}
    {% else %}
    {% assign headshot = person.headshot %}
    {% endif %}
    <div class="person">
      <p class="person"><a href="{{person.website}}"><img class="person" src="{{headshot}}"/></a></p>
      <p class="person"><a href="{{person.website}}">{{person.name}}</a></p>
      <p class="person">{{person.role}}</p>
      <p class="person">{{person.affiliation}}</p>
    </div>
  {% endfor %}
</div>

### --- German Research Center for Artificial Intelligence (DFKI) ---

<div class="people">
  {% for person in site.data.people.dfki %}
    {% if person.headshot == ""%}
    {% assign headshot = "/assets/imgs/gigachad.jpg" %}
    {% else %}
    {% assign headshot = person.headshot %}
    {% endif %}
    <div class="person">
      <p class="person"><a href="{{person.website}}"><img class="person" src="{{headshot}}"/></a></p>
      <p class="person"><a href="{{person.website}}">{{person.name}}</a></p>
      <p class="person">{{person.role}}</p>
      <p class="person">{{person.affiliation}}</p>
    </div>
  {% endfor %}
</div>

<!-- ### Max Planck Institute for Informatics -->
<style>
  h2, h3 {
   /* text-align: center; */
}

</style>

### --- Alumni ---

<div class="people">
  {% for person in site.data.people.alumni %}
    {% if person.headshot == ""%}
    {% assign headshot = "/assets/imgs/gigachad.jpg" %}
    {% else %}
    {% assign headshot = person.headshot %}
    {% endif %}
    <div class="person">
      <p class="person"><a href="{{person.website}}"><img class="person" src="{{headshot}}"/></a></p>
      <p class="person"><a href="{{person.website}}">{{person.name}}</a></p>
      <p class="person">{{person.role}}</p>
      <p class="person">{{person.affiliation}}</p>
    </div>
  {% endfor %}
</div>
