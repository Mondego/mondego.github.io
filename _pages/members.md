---
title: "Members"
layout: gridlay
excerpt: "Mondego -- Members"
sitemap: false
permalink: /members/
---

<h2 style="font-family: 'Roboto', sans-serif; font-weight: 500; font-size: 32px;">Principal Investigator</h2>
<br>
<div class="row">
  <div class="col-sm-4 clearfix">
  <img src="https://ics.uci.edu/~lopes/pics/Lopes3-square-2.jpg" class="img-responsive" width="80%" style="float: center" />
  <br>
  <h4><a href="https://ics.uci.edu/~lopes/" target="_blank">Cristina Videira Lopes</a></h4>
  <strong>Chancellor's Professor</strong><br>
  <a href="https://www.informatics.uci.edu/" target="_blank">Department of Informatics</a><br>
  <a href="http://isr.ics.uci.edu/" target="_blank">Institute for Software Research</a><br>
  <a href="http://www.ics.uci.edu/" target="_blank">Information and Computer Sciences</a><br>
  <a href="https://uci.edu/" target="_blank"> University of California, Irvine (UCI)</a><br>
  <i><lopes@ics.uci.edu></i><br>
  <a href="https://scholar.google.com/citations?hl=en&user=FaY_RgsAAAAJ&view_op=list_works&sortby=pubdate" target="_blank"><img src="{{ site.url }}{{ site.baseurl }}/images/logo/scholar.png" width="40px" height="40x"></a>
  <a href="https://dblp.org/pid/l/CristinaVideiraLopes.html" target="_blank"><img src="{{ site.url }}{{ site.baseurl }}/images/logo/dblp.png" width="40px" height="40x"></a>

  </div>
<div class="col-sm-8"> 
<p align="justify">
It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters, as opposed to using 'Content here, content here', making it look like readable English. Many desktop publishing packages and web page editors now use Lorem Ipsum as their default model text, and a search for 'lorem ipsum' will uncover many web sites still in their infancy. Various versions have evolved over the years, sometimes by accident, sometimes on purpose (injected humour and the like).
</p> </div>
</div>


<h2 style="font-family: 'Roboto', sans-serif; font-weight: 500; font-size: 32px;">Members</h2>
<br>

{% assign number_printed = 0 %}
{% for member in site.data.members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/group-members/current_members/{{ member.photo }}"  width="128px" height="128px" style="float: left" />
  <h4><a href="{{ member.homepage }}" target="_blank">{{ member.name }}</a></h4>
  <i><b>{{ member.current_position }}</b></i> <br>
  <i><b>{{ member.current_organization }}</b></i> <br>
  <i>email: {{ member.email }}</i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}



<!-- PhD Students  -->

<h2 style="font-family: 'Roboto', sans-serif; font-weight: 500; font-size: 32px;">PhD Students</h2>
<br>

{% assign number_printed = 0 %}
{% for member in site.data.phd %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/group-members/phd/{{ member.photo }}"  width="128px" height="128px" style="float: left" />
  <h4><a href="{{ member.homepage }}" target="_blank">{{ member.name }}</a></h4>
  <i>{{ member.current_position }} </i> <br>
  <i>{{ member.current_organization }} </i> <br>
  <i>email: {{ member.email }}</i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<!-- PhD Students -->

<!-- Masters Students  -->

<h2 style="font-family: 'Roboto', sans-serif; font-weight: 500; font-size: 32px;">Masters Students</h2>
<br>

{% assign number_printed = 0 %}
{% for member in site.data.mphil %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/group-members/mphil/{{ member.photo }}"  width="128px" height="128px" style="float: left" />
  <h4><a href="{{ member.homepage }}" target="_blank">{{ member.name }}</a></h4>
  <i>{{ member.current_position }} </i> <br>
  <i>{{ member.current_organization }} </i> <br>
  <i>email: {{ member.email }}</i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<!-- M.Phil Students -->

<!-- Alumni -->
<h2 style="font-family: 'Roboto', sans-serif; font-weight: 500; font-size: 32px;">Alumni</h2>
<br>

{% assign number_printed = 0 %}
{% for member in site.data.alumni %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/group-members/alumni/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4><a href="{{ member.homepage }}" target="_blank">{{ member.name }}</a></h4>
  <i>{{ member.current_position }} </i> <br>
  <i>{{ member.current_organization }} </i> <br>
  <i>email: {{ member.email }}</i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<!-- Alumni -->




### Administrative Support
If you need to update your information,<a href="https://github.com/Mondego/mondego.github.io" target="_blank"> here</a> create a PR with the changes and feel free to contact <a href="https://mondego.ics.uci.edu/" target="_blank">Mondego Research Group @ UC Irvine</a>.
<br>
<br>
<br>
<style>
  @media (max-width: 420px) {.fa-ul::before{content: "\A";white-space: pre;}}
</style>