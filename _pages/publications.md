---
title: "IDSL - Publications"
layout: gridlay
excerpt: "IDSL -- Publications"
sitemap: false
permalink: /publications/
---


# Publications and Patents

## Group Highlights

(For a full list of publications see <a href="https://scholar.google.com/citations?user=llkzRAYAAAAJ&hl=en">Google Scholar</a> or <a href="https://orcid.org/0000-0002-5125-7741">ORCID</a>)
{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
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


## Patents
<ul>
	<a id="qmda_patent"></a>
	<li>Methods and Systems for Multilinear Discriminant Analysis Via Invariant Theory for Data Classification
		<a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/20230350973">(US 2023/0350973 A1</a>)<br/>
		<i>Inventors: Kayvan Najarian, Olivia Pifer Alge, Jonathan Gryak, Harm Derksen, Cristian Minoccheri</i></li>
	<li>Sequential Minimal Optimization Process for Learning Using Partially Available Privileged Information Techniques 
		<!--<a href="https://appft.uspto.gov/netacgi/nph-Parser?Sect1=PTO1&Sect2=HITOFF&p=1&u=/netahtml/PTO/srchnum.html&r=1&f=G&l=50&d=PG01&s1=20200250496.PGNR.">(US 2020/0250496 A1</a>)<br/>-->
		<a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/11531851">(US 11,531,851)</a><br/>
	<i>Inventors: Kayvan Najarian, Jonathan Gryak, Elyas Sabeti, Joshua Drews</i></li>
	<li>Tensor Amplification-based Data Processing 
		<a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/20210338171">(US 2021/0338171)</a><br/>
	<i>Inventors: Hendrikus Derksen, Neriman Tokcan, Kayvan Najarian, Jonathan Gryak</i></li>
	<li>Automatic Filter Pruning Technique for Convolutional Neural Networks 
		<a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/10936913">(US 10,936,913)</a><br/>
	<i>Inventors: Heming Yao, Kayvan Najarian, Jonathan Gryak</i></li>
	<li>Automated Optic Nerve Sheath Diameter Measurement 
		<a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/20210022631">(US 2021/0022631)</a><br/>
	<i>Inventors: Reza Soroushmehr, Kayvan Najarian, Venkatakrishna Rajajee, Kevin Ward, Jonathan Gryak, Craig A. Williamson, Mohamad H. Tiba</i></li>
	<li>Automated Anatomic and Regional Location of Disease Features in Colonoscopy Videos 
		<a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/20200364859">(US 2020/0364859)</a><br/>
	<i>Inventors: Kayvan Najarian, Heming Yao, Reza Soroushmehr, Jonathan Gryak, Ryan Stidham</i></li>
	<li>Systems and Methods for Predicting and Detecting a Cardiac Event 
		<a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/11154254">(US 11,154,254</a>,
		<a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/10786208">US 10,786,208)</a>,
		<a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/10463314">US 10,463,314)</a><br/>	
	<i>Inventors: Kayvan Najarian, Harm Derksen, Zhi Li, Jonathan Gryak, Pujitha Gunaratne</i></li>
</ul>

<!-- 
## Full List of publications

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
-->
