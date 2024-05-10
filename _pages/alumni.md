---
title: "ETE Alumni"
layout: gridlay
excerpt: "ETE Alumni Profiles"
sitemap: false
permalink: /alumni/
---

# Alumni Profiles

 **We are  looking for new PhD students, Postdocs, and Master students to join the team** [(see openings)]({{ site.url }}{{ site.baseurl }}/vacancies) **!**


Jump to [industry/govt.](#industry/govt.), [master's and phd students](#Master's-and-PhD-Students), [academician](#academician), [administrative support](#administrative-support).

## Industry/Govt.
{% assign number_printed = 0 %}
{% for member in site.data.alumni_industry %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4><a href="{{member.url}}">{{ member.name }}</a></h4>
  <i>{{ member.edu1 }} {{ member.edu2 }}</i> <br>
  {% if member.number_emp == 1 %}
  <b>Now</b>: {{ member.now }}<br>
  <b>Expertise</b>: {{ member.expert}}<br>
  {% endif %}

  {% if member.number_emp == 2 %}
  <b>Now</b>: {{ member.now }}<br>
  <b>Previous</b>: {{ member.prev }}<br>
  <b>Expertise</b>: {{ member.expert }}<br>
  {% endif %}
 
  
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 | markdownify}} </li>
  <li> {{ member.education2 | markdownify}} </li>
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





## Master's and PhD Students

{% assign number_printed = 0 %}
{% for member in site.data.alumni_higher_study %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4><a href="{{member.url}}">{{ member.name }}</a></h4>
  <i>{{ member.edu1 }} {{ member.edu2 }}</i> <br>
  {% if member.number_emp == 1 %}
  <b>Now</b>: {{ member.now }}<br>
  <b>Research</b>: {{ member.expert}}<br>
  {% endif %}

  {% if member.number_emp == 2 %}
  <b>Now</b>: {{ member.now }}<br>
  <b>Research</b>: {{ member.expert }}<br>
  <b>Previous</b>: {{ member.prev }}<br>
  {% endif %}
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

## Academician

{% assign number_printed = 0 %}
{% for member in site.data.alumni_academic %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4><a href="{{member.url}}">{{ member.name }}</a></h4>
  <i>{{ member.edu1 }} {{ member.edu2 }}</i> <br>
  {% if member.number_emp == 1 %}
  <b>Now</b>: {{ member.now }}<br>
  <b>Research</b>: {{ member.expert}}<br>
  {% endif %}

  {% if member.number_emp == 2 %}
  <b>Now</b>: {{ member.now }}<br>
  <b>Previous</b>: {{ member.prev }}<br>
  <b>Research</b>: {{ member.expert }}<br>
   
  {% endif %}
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




## Administrative Support
<a href="mailto:Rijsewijk@Physics.LeidenUniv.nl">Ellie van Rijsewijk</a> is helping us (and other groups) with administration.
