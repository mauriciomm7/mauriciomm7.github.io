---
layout: archive
author_profile: true
permalink: /learn/
title: "Learning Resources"
---
<!-- 
[ ] ADD Literature Categories "Judicial Politics", "Comparative Politics", "European Politics", 
[ ] CREATE HTML Template for Methods docs
[ ] CREATE HTML Template for Literature docs 
    This should be more narrative-like with hyperlinks to a #section in a page contains summaries (copy pasted from notes).
[ ] CREATE HTML Template for Mathviz docs
[ ] ADD page with all summaries of each paper.
-->
This page is work in progress, I am planning to transfer the accomulated knowedlege-base from my Obsidian notes into a digestiable and systemtized format here. However, this is a long term project and will take some time.


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

***

This is test for using footones and wirting text after [^1]

[^1]: Footnote test.
