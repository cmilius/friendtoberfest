---
layout: home
---

This event is a celebration. It is the epitomy of gemütlichkeit (a German-language word used to convey the idea of a state or feeling of warmth, friendliness, and good cheer) to celebrate our friendship.

{% assign event = site.events | where: "title", "8th Annual Friendtoberfest" | first %}

{% include event-card.html
    banner=event.banner
    name=event.title
    location=event.location
    date=event.date
    excerpt=event.excerpt
    url=event.url
%}
