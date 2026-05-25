---
title: Courses
layout: landing
description: 'gisma spatial science resources'
image: assets/images/gisma-30.jpg
nav-menu: true
---
<style>
img {
  display: block;
  max-width:450px;
  max-height:450px;
  justify-content: center;
  align-items: center;
  width: auto;
  height: auto;
}
</style>

<!-- Main -->
<div id="main">

<!-- One -->
<section id="one">
<div class="inner">
<header class="major">
<h1>About gisma courses</h1>
</header>
<p>
The courses are regular courses in the Bachelor's and Master's programmes in Geography at the University of Marburg. They are offered by the Geoinformation Science Lab Marburg (gisma), which provides access to various teaching and research content from the Spatial Science Resources working group at the <a href="https://www.uni-marburg.de/en/fb19">Department of Geography</a>, <a href="https://www.uni-marburg.de/en">Marburg University</a>.

The course content is developed and hosted on <i class="fa fa-github"></i> <a href="https://github.com/gisma-courses/">GitHub</a>.

The responsibility for the content rests with the instructors. Statements, opinions and/or conclusions are those of the instructors and do not necessarily reflect the opinion of the representatives of Marburg University.
</p>
</div>
</section>


<section id="two" class="spotlights">
<div class="inner">
<header class="major">
<h1>{{ site.data.courses.regular.title }}</h1>
<h2>{{ site.data.courses.regular.subtitle }}</h2>
</header>
</div>

{% for course in site.data.courses.regular.items %}
{% include course-card.html course=course %}
{% endfor %}

</section>


<section id="three" class="spotlights">
<div class="inner">
<header class="major">
<h1>{{ site.data.courses.former.title }}</h1>
<h2>{{ site.data.courses.former.subtitle }}</h2>
</header>
</div>

{% for course in site.data.courses.former.items %}
{% include course-card.html course=course %}
{% endfor %}

</section>


<section id="four" class="spotlights">
<div class="inner">
<header class="major">
<h1>{{ site.data.courses.back_catalogue.title }}</h1>
<h2>{{ site.data.courses.back_catalogue.subtitle }}</h2>
</header>
</div>

{% for course in site.data.courses.back_catalogue.items %}
{% include course-card.html course=course %}
{% endfor %}

</section>

</div>

The focus is on reproducible scientific method training and education in the fields of environmental informatics, GIS, remote sensing and modelling.
