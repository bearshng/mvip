---
title: "Secure Learning and Control Lab - Team"
layout: gridlay
excerpt: "Team members"
sitemap: false
permalink: /team/
---

<style>

.button {
    clear: left;
    background-color: #4CAF50; /* Green */
    border: none;
    color: white;
    padding: 4px 20px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 12px;
    margin: 4px 2px;
    -webkit-transition-duration: 0.4s; /* Safari */
    transition-duration: 0.4s;
    cursor: pointer;
}

.black {
    background-color: white;
    color: black;
    border: 2px solid #555555;
}

</style>

# 组内成员

 **拟招2025年秋季入学硕士研究生2-3名，欢迎计算机、软件、电子、控制、物理、数学等相关专业学生通过邮件或电话联系。** [(招生信息见)]({{ site.url }}{{ site.baseurl }}/openings) **!**


<!-- Jump to [staff](#staff), [master and bachelor students](#master-and-bachelor-students).
{::comment}
, [alumni](#alumni), [lab visitors](#lab-visitors).
{:/comment}
 -->

## 教师
{% for member in site.data.team_members %}

<div class="row">

<div class="col-sm-12 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="15%" style="float: left" />
  
  <div style='margin-left:20%;'>
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }} <!--<br>email: <{{ member.email }}></i> -->
  
  <p style="font-size:.8em">{{ member.short_bio }}</p>
  </div>

  <p style="clear:both;"></p>
  <button class="button black" onclick="window.location.href='{{ member.website }}'" type="button">
  {{ member.name }}'s Personal Website</button>

</div>

</div>


{% endfor %}



## 在校生



{% assign number_printed = 0 %}
{% for member in site.data.alumni_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
 <br> {{ member.position }}
 <br> 本科: {{member.undergraduate}}
 <br> 研究方向: {{member.topics}}
<br> 成果: {{member.publications}}
  <ul style="overflow: hidden">

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %} 


## 毕业学生
<div class="row">

{::comment}
<div class="col-sm-4 clearfix">
<h4>Visitors</h4>
{% for member in site.data.alumni_visitors %}
{{ member.name }}
{% endfor %}
</div>
{:/comment}


<div class="col-sm-12 clearfix">
<h4>硕士研究生</h4>
{% for member in site.data.alumni_msc %}
{{ member.name }}
<i>{{ member.info }}</i>
{% endfor %}
</div>


<div class="col-sm-4 clearfix">
<h4>本科生</h4>
{% for member in site.data.alumni_bsc %}
{{ member.name }}
<i>{{ member.info }}</i>
{% endfor %}
</div>

</div>

