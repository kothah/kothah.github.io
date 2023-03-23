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
<i>{{ publi.link_main.display }}, <a href="{{ publi.link_main.url }}" target="_blank">[Link]</a></i>
<br>
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
1. A. Kopaničáková, **H. Kothari**, R. Krause<br>
   [Nonlinear Field-split Preconditioners for Solving Monolithic Phase-field Models of Brittle Fracture](https://doi.org/10.1016/j.cma.2022.115733)<br>
   _Computer Methods in Applied Mechanics and Engineering_, 403:115733, **2023**<br>
   DOI: 10.1016/j.cma.2022.115733
1. **H. Kothari**, R. Krause<br>
   [A generalized multigrid method for solving contact problems in Lagrange multiplier based unfitted Finite Element method](https://doi.org/10.1016/j.cma.2022.114630)<br>
   _Computer Methods in Applied Mechanics and Engineering_, 392:114630, **2022**<br>
   DOI: 10.1016/j.cma.2022.114630
1. **H. Kothari**, R. Krause<br>
   [A Multigrid Method for a Nitsche-based Extended Finite Element Method](https://doi.org/10.51375/IJCVSE.2021.1.8)<br>
   _International Journal of Computing and Visualization in Science and Engineering_, **2021**<br>
   DOI: 10.51375/IJCVSE.2021.1.8

## Conference Proceedings
1. **H. Kothari**, A. Kopaničáková, R. Krause<br>
   [A Multigrid Preconditioner for Jacobian-free Newton-Krylov Methods](http://www.ddm.org/DD26/proceedings/343.pdf)<br>
   In Domain Decomposition Methods in Science and Engineering XXVI. Lecture Notes in Computational Science and Engineering, vol 145. Springer, **2023**<br>
   DOI: 10.1007/978-3-030-95025-5_38 
1. **H. Kothari**, R. Krause<br>
   [Multigrid and saddle-point preconditioners for unfitted finite element modelling of inclusions](https://doi.org/10.23967/wccm-eccomas.2020.211)<br>
   In Proceedings of the $14^{th}$ World Congress on Computational Mechanics (WCCM) European Community on Computational Methods in Applied Sciences (ECCOMAS) Congress 2020, **2021**<br>
   DOI: 10.23967/wccm-eccomas.2020.211

## Thesis
* [Multilevel solution strategies for unfitted finite element method](https://susi.usi.ch/usi/documents/319417)<br> _PhD thesis_, Università della Svizzera italiana, **2020**
* [Parallelisation of a Spectral Element Solver](https://www.ics.usi.ch/images/kothari/kothari_master_thesis.pdf)<br> _Master thesis_, TU Bergakademie Freiberg, **2014**
