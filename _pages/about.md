---
layout: minimal
permalink: /
title: about
description: >
  [FILL IN] one-sentence description of who you are, used for link previews and search results.
---

<section id="about">
  <div class="about">
    <img class="about-photo" src="{{ '/assets/img/prof_pic.jpg' | relative_url }}" alt="{{ site.first_name }} {{ site.last_name }}">
    <div class="about-body">
      <h1>{{ site.first_name }} {{ site.last_name }}</h1>
      <p class="about-affiliation">[FILL IN: title/position], [FILL IN: institution]</p>
      <p class="about-bio">
        [FILL IN] Write one paragraph covering who you are, your position, and your
        research interests — e.g. "I am a PhD student at &lt;institution&gt; working on
        &lt;research area&gt;. My research focuses on &lt;specific problems/methods&gt;.
        Before that, I &lt;brief background&gt;." Keep it to 3-5 sentences.
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
