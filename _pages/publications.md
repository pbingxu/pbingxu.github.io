---
title: "PolyU GNSS Signal Processing - Publications"
layout: gridlay
excerpt: "PolyU GNSS Signal Processing - Publications."
sitemap: false
permalink: /publications/
---


## Research grants

As the role of **PI**:<br> 
- Research on direct position estimation based GNSS and 5G positioning and GNSS/5G deep integration mechanism, 1 Jan 2022~31 Dec 2024, NSFC for Young Scholar 國家自然科學基金委員會青年科學基金項目<br>

- Research on GNSS Vector Tracking based Anti-multipath Mechanism in Urban Environment, 廣東省基礎與應用基礎研究項目, 1 Jan 2022~31 Dec 2024<br>

- Security reinforcement for high-precision fusion positioning, 1 Dec 2021 ~ 30 Sep 2024, Huawei Technologies Co. Ltd. (Collaborative) <br>

- A-GNSS Based Direct Position Estimation: Modelling, Implementation and Performance Assessment, 15 Mar 2021~14 Mar 2023, PolyU Start-up Fund for RAPs under the Strategic Hiring Scheme <br>

As the role of **Co-PI**: <br>
- Reliable Multiagent Collaborative Global Navigation Satellite System Positioning for Intelligent Transportation Systems, 2022~2024, RGC Research Impact Fund Scheme (RIF) <br>


As the role of **Co-I**: <br>
- Unlocking the potential of AI edge intelligence and cloud-edge computing for flexible robotic and facility control system, 2 Jul 2021 ~ 1 Jul 2023, Innovation and Technology Fund - Partnership Research Programme (ITF-PRP)<br>


- Ultra-Tightly Coupled GNSS/INS Integration for Smartphone, 25 Dec 2018 ~ 24 Jan 2020, 9.	Ultra-Tightly Coupled GNSS/INS Integration for Smartphone<br>

See my [CV]({{ site.baseurl }}/downloads/CV of XU BING - As of Feb 2022 - Website.pdf) for more details.




## Research highlights

(For a full list of publications, please see [below](#full-list-of-publications) or go to [Google Scholar](https://scholar.google.com/citations?user=DN78yRMAAAAJ&hl=en), [ORCID](https://orcid.org/0000-0003-3677-1109))

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





## Journal Papers
(*: Corresponding author)

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}


## Conference Papers

{% for publi in site.data.publist_conference %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
