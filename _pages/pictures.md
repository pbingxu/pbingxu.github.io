---
title: "PolyU GNSS Signal Processing - Pictures"
layout: piclay
excerpt: "PolyU GNSS Signal Processing -- Pictures"
permalink: /pictures/
---

# Gallery
{% assign number_printed = 0 %}
{% for pic in site.data.pictures_Leiden %}

{% assign even_odd = number_printed | modulo: 4 %}



  <div class="col-sm-3 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
  </div>

  {% assign number_printed = number_printed | plus: 1 %}

  {% if even_odd > 2 %}
    </div>
  {% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}




<p> &nbsp; </p>


