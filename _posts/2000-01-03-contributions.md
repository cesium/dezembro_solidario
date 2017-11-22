---
title: "Como contribuir"
bg: contributions
color: white
border-color: white
fa-icon: gift
---

{% for activity in site.data.agenda.contributions %}
  {% capture thecycle %}{% cycle 'even', 'odd' %}{% endcapture %}
  {% if thecycle == 'odd' %}
  <div class="activity">
    <div class="row activity-info-wrapper valign-wrapper">
      <div class="col m3 activity-img valign">
        <img  src="img/{{ activity.image }}" alt="{{ activity.title }}">
      </div>
      <div class="col m9 activity-info">
        <h3 class="activity-title"> {{ activity.title }} </h3>
        {% if activity.time %}
        <div class="col s12 activity-time">
          <i class="fa fa-clock-o"></i> <span> {{ activity.time }} </span>
        </div>
        {% endif %}
        {% if activity.place %}
        <div class="col s12 activity-place">
          <i class="fa fa-map-marker"></i> <span> {{ activity.place }} </span>
        </div>
        {% endif %}
        <p class="col m12 activity-desc"> {{ activity.text }} </p>
        {% if activity.typeform %}
        <a class="waves-effect waves-light btn bg-{{ page.border-color }}" href="{{ activity.typeform }}" target="blank">Inscrição</a>
        {% endif %}
      </div>
    </div>
  </div>
  {% else %}
  <div class="activity">
    <div class="row activity-info-wrapper valign-wrapper">
      <div class="col m3 activity-img valign img-mobile">
        <img src="img/{{activity.image}}" alt="{{activity.title}}">
      </div>
      <div class="col m9 activity-info">
        <h3 class="activity-title"> {{ activity.title }} </h3>
        {% if activity.time %}
        <div class="col s12 activity-time">
          <i class="fa fa-clock-o"></i> <span> {{ activity.time }} </span>
        </div>
        {% endif %}
        {% if activity.place %}
        <div class="col s12 activity-place">
          <i class="fa fa-map-marker"></i> <span> {{ activity.place }} </span>
        </div>
        {% endif %}
        <p class="col m12 activity-desc"> {{ activity.text }} </p>
        {% if activity.typeform %}
        <a class="waves-effect waves-light btn bg-{{ page.border-color }}" href="{{ activity.typeform }}" target="blank">Inscrição</a>
        {% endif %}
      </div>
      <div class="col m3 activity-img valign img-desktop">
        <img src="img/{{activity.image}}" alt="{{activity.title}}">
      </div>
    </div>
  </div>
  {% endif %}
{% endfor %}