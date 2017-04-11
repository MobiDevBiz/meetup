---
layout: page
title: Події
---

<div class="events-list list-group">  
{% for event in site.events %}
    <a class="list-group-item" href="{{ event.url }}" >
      <b>#{{ event.uuid }}, {% include date.html date=event.date %}, {{ event.category }}</b>. {{ event.title }}
      <div class="ripple-container"></div>
      </a>
{% endfor %}
</div> 
