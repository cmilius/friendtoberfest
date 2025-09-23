---
layout: page
title: Events
---

{% for event in site.events reversed %}

{% include event-card.html
    banner=event.banner
    name=event.title
    location=event.location
    date=event.date
    excerpt=event.excerpt
    url=event.url
%}

{% unless forloop.last %}
---
{% endunless %}

{% endfor %}
