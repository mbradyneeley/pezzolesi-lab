---
title: "Pezzolesi Lab - News"
layout: textlay
excerpt: "Pezzolesi Lab at UU."
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br>
<em>{{ article.headline }}</em></p>
{% endfor %}
