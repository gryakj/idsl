---
title: "News"
layout: textlay
excerpt: "Allan Lab at Leiden University."
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
 <p> <em>{{ article.date }} </em></p>
 <p> {{ article.headline}} </p>
{% endfor %}
