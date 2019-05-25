---
layout: page
title: 서울S치과의원
permalink: /dentist/
category1: 진료안내
category2: 의료진
published: true
frontpage: true
---
<div id="dentist">

<div class="row">
{% for person in site.data.dentist %}

  <div class="col-12 person">
    <div class="card">
      <div class="card-body">
        <div class="portrait" >
            <img onclick="window.open('{{ person.link }}');" src="{% if person.portrait %}{{site.url}}/img/{{ person.portrait}}{% elsif person.extportrait %}{{ person.extportrait }}{% else %}{{site.url}}/img/anonymous.jpg{% endif %}">
        </div>
        <div class="info">
          <h5 class="card-title">{{ person.name}} {{ person.jobtitle}}</h5>
          <p class="card-text">{{ person.specialty }}</p>
          <ul>
          {% for item in person.school %}
          <li>{{ item }}</li>
          {% endfor %}
          </ul>
          <ul>
          {% for item in person.cv %}
          <li>{{ item }}</li>
          {% endfor %}
          </ul>
        </div>
      </div>
    </div>
  </div>
{% endfor %}
</div>

</div>
