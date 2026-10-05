---
layout: minimal
permalink: /
title: about
description: >
  Shuai Zhu is a Research Engineer at RISE Research Institutes of Sweden and an industrial PhD student at Uppsala University, working on embedded AI and IoT networks.
---

<section id="about">
  <div class="about">
    <img class="about-photo" src="{{ '/assets/img/prof_pic.jpg' | relative_url }}" alt="{{ site.first_name }} {{ site.last_name }}">
    <div class="about-body">
      <h1>{{ site.first_name }} {{ site.last_name }}</h1>
      <p class="about-affiliation">Research Engineer, RISE Research Institutes of Sweden<br>Industrial PhD Student, Uppsala University</p>
      <p class="about-bio">
        I am a Research Engineer at RISE Research Institutes of Sweden and an industrial
        PhD student at Uppsala University, supervised by Prof. Thiemo Voigt, Prof. JeongGil Ko,
        and Dr. Fatemeh Rahimian. My research focuses on embedded AI and IoT networks. Before my PhD, I spent three years
        in industry as an Android engineer, working on both application development and the
        Android platform. I hold a double master's degree from KTH Royal Institute of
        Technology, Sweden, and Aalto University, Finland, and a bachelor's degree from
        Southeast University, China.
      </p>
      {% include social_links.liquid %}
    </div>
  </div>
</section>

<section id="news">
  <h2 class="section-label">News</h2>
  {% include news_list.liquid %}
</section>

<section id="publications" class="publications">
  <h2 class="section-label">Publications</h2>
  {% bibliography %}
</section>

<section id="service">
  <h2 class="section-label">Service</h2>
  <ul class="service-list">
    {% for item in site.data.service %}
      <li>
        <span>{{ item.role }}{% if item.org %}, {{ item.org }}{% endif %}</span>
        <span class="service-year">{{ item.year }}</span>
      </li>
    {% endfor %}
  </ul>
</section>
