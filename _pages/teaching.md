---
layout: page
permalink: /teaching/
title: teaching
description: materials for courses I currently teach or taught in the past.
nav: true
---

<div class="projects grid">

  {% assign sorted_projects = site.teaching | sort: "date" %}
  {% for project in sorted_projects %}
  <div class="grid-item">
    {% if teaching.redirect %}
    <a href="{{ project.redirect }}" target="_blank">
    {% else %}
    <a href="{{ project.url | relative_url }}">
    {% endif %}
      <div class="card hoverable">
        {% if project.img %}
        <img src="{{ project.img | relative_url }}" alt="project thumbnail">
        {% endif %}
        <div class="card-body">
          <h2 class="card-title">{{ project.title }}</h2>
          <p class="card-text">{{ project.description }}</p>
          <div class="row ml-1 mr-1 p-0">
            {% if project.github %}
            <div class="github-icon">
              <div class="icon" data-toggle="tooltip" title="Code Repository">
                <a href="{{ project.github }}" target="_blank"><i class="fab fa-github gh-icon"></i></a>
              </div>
              {% if project.github_stars %}
              <span class="stars" data-toggle="tooltip" title="GitHub Stars">
                <i class="fas fa-star"></i>
                <span id="{{ project.github_stars }}-stars"></span>
              </span>
              {% endif %}
            </div>
            {% endif %}
          </div>
        </div>
      </div>
    </a>
  </div>
{% endfor %}

</div>

---

**Teaching assignments:**

- HISP-S 150: _Elementary Spanish II_ (Fall 2016)

- HISP-S 200: _Second-year Spanish I_ (Fall 2017; Spring 2018)

- HISP-S 250: _Second-year Spanish II_ (Spring 2017; Fall 2019)

- HISP-S 280: _Spanish Grammar in Context_ (Spring 2020 - second half online)

- HISP-S 326: _Introduction to Hispanic Linguistics_ (Fall 2020 - hybrid; Spring 2021 - online)

- HISP-S 315: _Spanish in the Business World_ (Fall 2021)

- HISP-S 281: _Spanish Grammar in Context for Heritage Speakers_ (Spring 2022)

- HISP-S 308: _Composition and Conversation in Spanish_ (Fall 2022, Spring 2023)