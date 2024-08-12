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

## Meeting Schedule

Meeting slides are made available in members-only calendar invites.

[[Paper discussion spreadsheet](https://docs.google.com/spreadsheets/d/1mtKZQAroeNrVTtavV9VJvH0ZwKZs3IBPCw_X20zsDWw/edit?usp=sharing)]

### Autumn 2024 Meetings

- Time: 11:00am, Every Tuesday
- Place: TUAS 1596 and Zoom

## Announcements

- Autumn 2024 information session will be held in late August, exact date TBD.
- We are recruiting! Prospective research mentees are encouraged to apply [here](asdf).

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
