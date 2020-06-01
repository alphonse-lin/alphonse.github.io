---
title: Instrumental Analysis I
description: WCU Chem 370
layout: home
permalink: /devel/chem370/
---

<div class="card">
  {% for post in site.posts limit:1 %}
    <article class="post">

      <h1><a href="{{ site.baseurl }}/chem370/announcements">Announcements</a></h1>

      <div class="entry">
        {{ post.content }}
      </div>

      <a href="{{ site.baseurl }}/chem370/announcements" class="read-more">Read More</a>
    </article>
  {% endfor %}
</div>

<h1>Course Materials</h1>

<a class="homepage-button" href="{{site.baseurl}}/devel/chem370/assignments/submissions-monday.html">
  <i class="fa fa-paper-plane fa-lg"></i>
  assignment submissions
</a>

<div class="column">
<a class="homepage-button" href="{{site.baseurl}}/devel/chem370/syllabus">
<i class="fa fa-scroll fa-lg"></i>
lecture syllabus
</a>
<!-- <a class="homepage-button" href="{{site.baseurl}}/devel/chem370/schedule">
 <i class="fa fa-calendar-alt fa-lg"></i>
 lecture schedule
</a> -->
<a class="homepage-button" href="{{site.baseurl}}/devel/chem370/lectures">
  <i class="fa fa-chalkboard-teacher fa-lg"></i>
  lectures
</a>
<a class="homepage-button" href="{{site.baseurl}}/devel/chem370/instrument-tutorials">
  <i class="fa fa-digital-tachograph fa-lg"></i>
  instrument tutorials
</a>
<a class="homepage-button" href="{{site.baseurl}}/devel/chem370/chemistry">
  <i class="fa fa-atom fa-lg"></i>
  chemistry
</a>
</div>
<!-- <hr class="hr-line"> -->
<div class="column">
<a class="homepage-button" href="{{site.baseurl}}/devel/chem370/lab-manual">
    <i class="fa fa-vial fa-lg"></i>
    lab manual
</a>
<a class="homepage-button" href="{{site.baseurl}}/devel/chem370/data-processing">
    <i class="fa fa-chart-line fa-lg"></i>
    data processing
</a>
<a class="homepage-button" href="{{site.baseurl}}/devel/chem370/writing">
   <i class="fa fa-edit fa-lg"></i>
   writing
</a>
<a class="homepage-button" href="{{site.baseurl}}/devel/chem370/notebooks">
  <i class="fa fa-book-open fa-lg"></i>
  notebooks (move)
</a>
</div>
