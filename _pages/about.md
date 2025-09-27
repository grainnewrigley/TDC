---
permalink: /
title: "Two Degrees Cooler"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

<img src="https://grainnewrigley.github.io/TDC//images/Header-temporary.jpg" alt="Header Temporary">

## About Two Degrees Cooler

Two Degrees Cooler is a climate and sustainability education organisation, founded in 2021. Through social media and blog posts, our goal is to inspire the public to take an interest in environmental issues through science communication. Beginning as a blog, the project has expanded to social media, data analysis and projects like Spotlight. 

### Our Values

<ul>
<li>Accessible communication</li>
<li>Trustworthy sources</li>
<li>Science for everyone</li>
</ul>

### Our People

Grainne Wrigley is a data analyst and science communicator based in the UK. Coming from a background in physics, she noticed barriers to science particiaption like the 'genius' scientist stereotype, or needless use of technical terminology, which prevented the public from engaging with science. Two Degrees Cooler was created out of a desire to encourage people to learn about environmental issues that affect their local communities and empower them to get involved.


<div class="page__related-home">
  <div class="page__inner-wrap">
    <h4 class="page__related-title">Recent Posts</h4>
    <div class="grid__wrapper">
      {% for post in site.posts limit:4 %}
        {% include archive-single.html type="grid" %}
      {% endfor %}
    </div>
  </div>
</div>
