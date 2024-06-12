---
title: "PolyU PNT Signal Processing - Publications"
layout: gridlay
excerpt: "PolyU PNT Signal Processing - Publications."
sitemap: false
permalink: /publications/
---



## Research highlights

(For a full list of publications, please see [below](#journal-papers) or go to [Google Scholar](https://scholar.google.com/citations?user=DN78yRMAAAAJ&hl=en), [ORCID](https://orcid.org/0000-0003-3677-1109), [ResearcherID](https://publons.com/researcher/4635979/bing-xu/publications/))

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

## Current research projects

- Research on direct position estimation based GNSS and 5G positioning and GNSS/5G deep integration mechanism, 2022~2024<br>
- Security reinforcement for high-precision fusion positioning, 2021~2024<br>
- Research on GNSS Vector Tracking based Anti-multipath Mechanism in Urban Environment, 2022~2024<br>
- Development and verification of SLAM+RTK navigation technology for smartphones, 2023~2025<br>

<p> &nbsp; </p>
<p> &nbsp; </p>
## Journal Papers

#### 2024
{% for publi in site.data.publist_2024 %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}


#### 2023
{% for publi in site.data.publist_2023 %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}


#### 2022
{% for publi in site.data.publist_2022 %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}

#### 2021
{% for publi in site.data.publist_2021. %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}

#### 2020
{% for publi in site.data.publist_2020 %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}

#### 2019
{% for publi in site.data.publist_2019 %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}

#### 2018
{% for publi in site.data.publist_2018 %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}

#### 2017
{% for publi in site.data.publist_2017 %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}




## Conference Papers

{% for publi in site.data.publist_conference %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
