---
title: "Secure Learning and Control Lab - Funding"
layout: textlay
excerpt: "Secure Learning and Control Lab -- Funding."
sitemap: false
permalink: /funding/
---

<!-- # Our Funding
We are grateful to the following organizations that generously fund our activities:
- [Uppsala University](http://www.it.uu.se),
	- [UU Graduate School in Cybersecurity](http://www.it.uu.se/research/research-arenas/security/graduate_school), an initiative from the Department of Information Technology,
- [Knut and Alice Wallenberg Foundation](https://kaw.wallenberg.org/) ([Wallenberg Academy Fellow](https://kaw.wallenberg.org/en/andre-teixeira)), 
- [Swedish Research Council](https://www.vr.se), 
- [Swedish Foundation for Strategic Research](https://strategiska.se) ([Future Research Leaders 7](https://strategiska.se/en/research/ongoing-research/framtidens-forskningsledare-7/)),
- [Swedish Energy Agency](https://www.energimyndigheten.se/en/),
- [Sweden's Innovation Agency](https://www.vinnova.se/en/),
- [eSSENCE-SciLife Graduate School in Data-Intensive Science](https://essenceofescience.se/graduate-school/).

<div class="row">

<div class="col-sm-2 clearfix vcenter">
<img src="{{ site.url }}{{ site.baseurl }}/images/logopic/UU_logo_4f125px.png" style="width: 125px">

</div>

<div class="col-sm-2 clearfix vcenter">
<img src="{{ site.url }}{{ site.baseurl }}/images/logopic/KAW_Logotype_Large.png" style="width: 125px">

</div>

<div class="col-sm-2 clearfix vcenter">
<img src="{{ site.url }}{{ site.baseurl }}/images/logopic/svart_fyrkant_eng.png" style="width: 120px">

</div>

<div class="col-sm-2 clearfix vcenter">
<img src="{{ site.url }}{{ site.baseurl }}/images/logopic/ssf_gb_rgb-300x247.png" style="width: 124px">
</div>
</div>

<div class="row">

<div class="col-sm-2 clearfix vcenter">
<img src="{{ site.url }}{{ site.baseurl }}/images/logopic/energimyndigheten_engelsklogo_rgb.png" style="width: 120px">
</div>

<div class="col-sm-2 clearfix vcenter">
<img src="{{ site.url }}{{ site.baseurl }}/images/logopic/Vinnova_green_payoff_ENG_RGB.png" style="width: 120px">
</div>

<div class="col-sm-2 clearfix vcenter">
<img src="{{ site.url }}{{ site.baseurl }}/images/logopic/LOGO_essence.png" style="width: 120px">
</div>


</div>

Their funding supports our work in research, education, and outreach, not the least through our scientific projects. -->

### 在研项目

{% for project in site.data.project %}

{% if project.ongoing == 1 %}
<div class="row">
<div class="well">

#### {{ project.title }} ({{ project.period}})

**项目来源:** {{ project.agency}}

**金额:** {{ project.money}}

**负责人:** {{project.lead}}

<!-- **执行时间:** {{project.period}} -->

<!-- **USLC Members:** {{project.member}} -->

<!-- <a data-toggle="collapse" href="#{{project.key}}-bib"  class="btn-abstract" style="text-decoration:none; color:#ebebeb; hover:#ebebeb;" role="button" aria-expanded="false">**Popular Abstract**</a>
<div class="collapse" id="{{project.key}}-bib"><div class="well-abs">
{{ project.summary }}
</div> </div>-->
</div>
</div>

{% endif %}

{% endfor %}


<h4><a href="{{ site.url }}{{ site.baseurl }}/allprojects.html">... 所有项目</a></h4>
