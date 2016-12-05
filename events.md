---
layout: page
title: Події
---

<div class="events-list list-group">  
{% for event in site.events %}
    <a class="list-group-item" href="{{ event.url }}" >
      <b>#{{ event.uuid }}, {{ event.date | date: "%d.%m.%Y" }}, {{ event.category }}</b>. {{ event.title }}
      <div class="ripple-container"></div>
      </a>
{% endfor %}
</div> 
