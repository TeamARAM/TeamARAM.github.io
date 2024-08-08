---
title: "Publications"
mytitle: "Publications"
layout: splash
# permalink: /splash-page/
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/publications.jpg
  # actions:
  #   - label: "Join Us"
  #     url: "/joinus/"
# excerpt: "Meeting time: 11:00am Every Tuesday, TUAS 1596 and Zoom"
---

## Conference Papers

<style>
div.paper {
  display: flex;
  flex-wrap: wrap;
  align-items: left;
  justify-content: center;
  padding: 10px 0;
}

img.paper-image {
  width: 180px;
  height: 180px;
}

div {
  /* border: 1px solid black; */
}

div.paper-desc {
  width: 1030px;
  margin-left: auto;
  /* margin-right: 15px; */
  /* justify-content: right; */
}

p.paper {
  /* text-align: center; */
  margin: 3px 0;
}


</style>

{% for year in site.data.publications.years %}

### --- {{year.year}} ---

<div class="papers">
{% for paper in year.papers %}
  <div class="paper">
    <div class="paper-image">
      <img src="{{paper.image}}" class="paper-image" />
    </div>
    <div class="paper-desc">
      <p class="paper"><b>{{paper.title}}</b></p>
      <p class="paper">{{paper.authors}}</p>
      <p class="paper"><i>{{paper.venue}}</i></p>
      <p class="paper">[<a href="{{paper.website}}">Project website</a>]</p>
    </div>
  </div>
{% endfor %}
</div>
{% endfor %}

## Theses

### --- 2023 ---

<div class="papers">
{% for paper in site.data.publications.theses.year2023 %}
  <div class="paper">
    <div class="paper-image">
      <img src="{{paper.image}}" class="paper-image" />
    </div>
    <div class="paper-desc">
      <p><b>{{paper.title}}</b></p>
      <p>{{paper.authors}}</p>
    </div>
  </div>
{% endfor %}
</div>
