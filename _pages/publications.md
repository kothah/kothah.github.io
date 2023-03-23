---
layout: publications
title: "Publications"
permalink: /publications/
author_profile: true
---
## Submitted manuscripts
<ul class="preprint_list">
{% assign number_printed = 0 %}
{% for publi in site.data.publication_list %}
{% if publi.type == "preprint" %}

<li ><p>
<b>{{ publi.title }}</b> ({{ publi.year }})
<br>{{ publi.authors }}<br>
<a href="javascript:toggleBibtex('{{ publi.label }}')">[BibTeX]</a>
<a href="{{ publi.link_pre.url }}" target="_blank">[Preprint]</a> 
</p>
<div id="bib_{{ publi.label }}" class="bibtex noshow">
<pre>
{{ publi.bibtex }}
</pre>
</div>
</li>

{% endif %}
{% endfor %}

</ul>

## Journal articles
<!-- Generated from JabRef by PubList by Truong Nghiem at 11:44 on 2015.09.10. -->
<ul class="biblist">

{% assign number_printed = 0 %}
{% for publi in site.data.publication_list %}
{% if publi.type == "journal" %}

<li ><p>
<b>{{ publi.title }}</b> ({{ publi.year }})
<br>{{ publi.authors }}<br>
<i>{{ publi.link_main.display }}</i>
<br> 
<a href="{{ publi.link_main.url }}" target="_blank">[Link]</a>
<a href="javascript:toggleBibtex('{{ publi.label }}')">[BibTeX]</a>
<a href="{{ publi.link_pre.url }}" target="_blank">[PDF]</a> 
</p>
<div id="bib_{{ publi.label }}" class="bibtex noshow">
<pre>
{{ publi.bibtex }}
</pre>
</div>
</li>

{% endif %}
{% endfor %}

</ul>

## Conference Proceedings
<ul class="biblist">

{% assign number_printed = 0 %}
{% for publi in site.data.publication_list %}
{% if publi.type == "inproceeding" %}

<li ><p>
<b>{{ publi.title }}</b> ({{ publi.year }})
<br>{{ publi.authors }}<br>
<i>{{ publi.link_main.display }}</i>
<br> 
<a href="{{ publi.link_main.url }}" target="_blank">[Link]</a>
<a href="javascript:toggleBibtex('{{ publi.label }}')">[BibTeX]</a>
<a href="{{ publi.link_pre.url }}" target="_blank">[PDF]</a> 
</p>
<div id="bib_{{ publi.label }}" class="bibtex noshow">
<pre>
{{ publi.bibtex }}
</pre>
</div>
</li>

{% endif %}
{% endfor %}

</ul>

## Thesis
* [Multilevel solution strategies for unfitted finite element method](https://susi.usi.ch/usi/documents/319417)<br> _PhD thesis_, Università della Svizzera italiana, **2020**
* [Parallelisation of a Spectral Element Solver](https://www.ics.usi.ch/images/kothari/kothari_master_thesis.pdf)<br> _Master thesis_, TU Bergakademie Freiberg, **2014**
