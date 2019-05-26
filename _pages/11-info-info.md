---
layout: page
title: 서울S치과 진료안내
permalink: /info/
category1: 진료안내
category2: 진료안내
frontpage: true
---
<h4>진료시간</h4>
<div class="row hours">
<div class="col-12">
<div class="row header {% cycle 'rowColor1', 'rowColor2' %}">
  <div class="col-2">요일</div>
  <div class="col-5">오전</div>
  <div class="col-5">오후</div>
</div>

{% for day in site.data.hours %}
<div class="row {% cycle 'rowColor1', 'rowColor2' %}">

  <div class="col-2">{{ day.day }}</div>
  {% if day.day contains "목" or day.day contains "일" %}
  <div class="col-10">휴무</div>
  {% else %}
  <div class="col-5 morning">{{ day.morning }}</div>
  <div class="col-5 afternoon">{{day.afternoon}}</div>
  {% endif %}

</div>
{% endfor %}

</div></div>

<p></p>

<h4>예약/문의</h4>

<p>예약을 하고 오시면 대기시간이 짧아집니다.</p>
<p><i style="width: 1.5em;" class="fa fa-phone"></i><a href="tel:+82222027528">02-2202-7528</a></p>

<img src="http://www.sorthodontic.com/image/m1_s3_img1.gif">
<img src="http://www.sorthodontic.com/image/m1_s3_img2.gif">
