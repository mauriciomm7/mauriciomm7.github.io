---
layout: archive
author_profile: true
permalink: /learn/
title: "Learning Resources"
---
<!-- 
[ ] ADD Literature Categories "Judicial Politics", "Comparative Politics", 
[ ] CREATE HTML Template for Methods docs
[ ] CREATE HTML Template for Literature docs
[ ] CREATE HTML Template for Mathviz docs
-->

<div class="container">
  <h2>Methods</h2>
  <ul>
    {% for doc in site.docs %}
      {% if doc.category == 'methods' %}
        <li><a href="{{ doc.url }}">{{ doc.title }}</a></li>
      {% endif %}
    {% endfor %}
  </ul>
</div>

<div class="container">
  <h2>Literature</h2>
  <ul>
    {% for doc in site.docs %}
      {% if doc.category == 'literature' %}
        <li><a href="{{ doc.url }}">{{ doc.title }}</a></li>
      {% endif %}
    {% endfor %}
  </ul>
</div>

<div class="container">
  <h2>MathViz</h2>
  <ul>
    {% for doc in site.docs %}
      {% if doc.category == 'mathviz' %}
        <li><a href="{{ doc.url }}">{{ doc.title }}</a></li>
      {% endif %}
    {% endfor %}
  </ul>
</div>

This is test [^1]

[^1]: Footnote test.
