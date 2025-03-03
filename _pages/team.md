---
title: "Cui Lab - Team"
layout: gridlay
excerpt: "Cui Lab: Team members"
sitemap: false
permalink: /team/
---

# Group Members

 **We are looking for passionate Postdoc, Assistant Investigator and Research Assistant to join the team** [(see Positions)]({{ site.url }}{{ site.baseurl }}/positions) **!**


<!-- Jump to [staff](#staff), [master and bachelor students](#master-and-bachelor-students), [alumni](#alumni), [administrative support](#administrative-support), [lab visitors](#lab-visitors). -->

### Principal Investigator
<div style="padding-left: 0px;">
<div class="well"  style="height: 368px; width: 845px">
<img src="/images/cuiguizhong.jpg" width="25%" style="float: left;"/>
<h4><strong>&nbsp;&nbsp;&nbsp;&nbsp;Guizhong Cui(崔桂忠)<strong></h4>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;cui_guizhong@gzlab.an.cn</p>
<!-- <p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<b>Principal Investigator</b></p> -->
<ul style="list-style-type:square; overflow: hidden">
<li>2022-present, Principal Investigator, Department of Basic Research, Guangzhou National Laboratory</li>
<li>2022-present, Professor, School of Basic Medical Sciences, Guangzhou Medical University</li>
<li>2019-2022, Associate Professor, Center of Cell Lineage and Atlas, Bioland Laboratory</li>
<li>2014-2019, Ph.D, Shanghai Institute of Biochemistry and Cell Biology, Chinese Academy of Sciences</li>
<li>2010-2014, B.S., College of Innovation and Experiment, College of Life Sciences, Northwest A&F University</li>
</ul>
</div>
</div>

<!-- <div class="row"> </div> -->

### Staff and Students
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-3 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="80%" style="float: top" />
  <h5>{{ member.name }}</h5>
  <p>{{ member.info }}</p>
  <p>{{ member.email }}</p>
  {% if member.area %}
  <p>{{ member.area }}</p>
  {% endif %}
  
</div>

{% assign number_printed = number_printed | plus: 1 %}   

{% if even_odd == 3 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd != 0 %}
</div>
{% endif %}




