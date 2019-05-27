---
layout: page
title: 서울S치과 진료안내
permalink: /info/
category1: 진료안내
category2: 진료안내
frontpage: true
---
<p>서울S치과는 <b>서울대학교 치과병원</b> 협력의료기관입니다.<BR>
서울대학교 치과대학을 졸업하고 서울대학교 치과병원에서 수련을 마친 보건복지부 인증 전문의가 최상의 진료를 합니다.</p>
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
  <div class="col-10">휴진</div>
  {% else %}
  <div class="col-5 morning">{{ day.morning }}</div>
  <div class="col-5 afternoon">{{day.afternoon}}</div>
  {% endif %}

</div>
{% endfor %}

</div></div>

<p></p>

<h4>예약/문의</h4>

<p>서울S치과 방문 전 예약을 하시면 대기시간이 짧아집니다.</p>
<p><i style="width: 1.5em;" class="fa fa-phone"></i><a href="tel:+82222027528">02-2202-7528</a><a href="tel:+82222027529">~9</a> | <i style="width: 1.5em;" class="fa fa-fax"></i><a href="tel:+82222027527">02-2202-7527</a></p>

<img src="http://www.sorthodontic.com/image/m1_s3_img1.gif">
<img src="http://www.sorthodontic.com/image/m1_s3_img2.gif">
