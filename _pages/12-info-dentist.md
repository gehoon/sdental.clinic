---
layout: page
title: 서울S치과의원
permalink: /dentist/
category1: 진료안내
category2: 의료진
published: true
frontpage: true
---

<div class="row d-flex justify-content-center" id="dentist">

{% for person in site.data.dentist %}

<div class="card">
  <img src="{% if person.portrait %}{{site.url}}/img/{{ person.portrait}}{% elsif person.extportrait %}{{ person.extportrait }}{% else %}{{site.url}}/img/anonymous.jpg{% endif %}" class="card-img-top" alt="...">
  <div class="card-body">
    <h5 class="card-title">{{ person.name}} {{ person.jobtitle}}</h5>
    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>

{% endfor %}

</div>
