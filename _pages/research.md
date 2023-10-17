---
title: "IDSL - Research"
layout: gridlay
excerpt: "IDSL - Research"
sitemap: false
permalink: /research/
---

# Research Focus

The Interdisciplinary Data Science Lab (IDSL) works to solve problems in biomedical informatics and computer science by developing novel artificial intelligence/machine learning methods that can leverage a problem's underlying morphology and work within its operational limitations.
 
Most recently, we have focused on the development of **Nonlinear Algebraic Data Analysis**, which leverages methodologies from  *tensor analysis*, *numerical algebraic geometry*, *deep neural networks*, and *invariant theory*. The application of nonlinear algebraic methods to data analysis has the potential to more *accurately* and *faithfully* model *complex, real-world data*.

## Research Areas

{% assign number_printed = 0 %}
{% for publi in site.data.research %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/respic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
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

<p> &nbsp; </p>