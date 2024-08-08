---
title: "Home"
mytitle: "Team ARAM: Animation, Robotics, and Machine Learning"
layout: splash
# permalink: /splash-page/
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/coffee.jpg
  actions:
    - label: "Join Us"
      url: "/joinus/"
excerpt: "Meeting time: 11:00am Every Tuesday, TUAS 1596 and Zoom"
---

## Announcements

- Fall 2024 information session will be held in late August, exact date TBD.
- We are recruiting! Prospective research mentees are encouraged to apply [here](asdf).

## Meeting Schedule

Meeting slides are made available in members-only calendar invites.

### Fall 2024

- 2024-08-13
  - Paper discussion: [RvS: What is Essential for Offline RL via Supervised Learning?](https://arxiv.org/abs/2112.10751) (Niko)
  - Project updates

### Summer 2024

- 2024-07-23
  - Paper discussion: (Nami)
- 2024-07-16
  - Paper discussion: (Noshaba)
- 2024-07-09
  - Paper discussion: (Nam Hee)

## People

### Aalto University

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
    <div class="person">
      <p class="person"><a href="{{person.website}}"><img class="person" src="{{person.headshot}}"/></a></p>
      <p class="person"><a href="{{person.website}}">{{person.name}}</a></p>
      <p class="person">{{person.role}}</p>
      <p class="person">{{person.affiliation}}</p>
    </div>
  {% endfor %}
</div>

### German Research Center for Artificial Intelligence (DFKI)

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

### Alumni

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
