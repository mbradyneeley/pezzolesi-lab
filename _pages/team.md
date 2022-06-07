---
title: "Pezzolesi Lab - Team"
layout: gridlay
excerpt: "Pezzolesi Lab: Team members"
sitemap: false
permalink: /team/
---

# Team Members
(Please click the name below for the lab member's profile)

{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if member.group == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive rounded" width="175" margin-left="auto" margin-right="auto" display="block"/>
  <h4><a href="{{ member.url }}" class="off">{{ member.name }}</a></h4>
  <i>{{ member.info }}</i>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

---

## Alumni

{% for member in site.data.team_members %}
{% if member.group == 8 %}

<i class="alumni1">{{ member.name }}</i><br>
<i class="alumni2">{{ member.info }} ({{ member.year }}</i>) {% if member.current %} 
<i class="alumni2">Current: {{ member.current }}</i> {% if member.extlink %} <a class="alumni2" style="padding-left: 0px;" href="{{ member.extlink }}">(Link)</a>
{% endif %}
{% endif %}

{% endif %}
{% endfor %}

---
