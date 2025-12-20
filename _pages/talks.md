---
layout: archive
title: "Talks and presentations"
permalink: /talks/
author_profile: true
---

{% if site.talkmap_link == true %}
<p style="text-decoration:underline;"><a href="/talkmap.html">See a map of all the places I've given a talk!</a></p>
{% endif %}

{% assign talks = site.data.talks | sort: "year" | reverse %}
{% assign grouped = talks | group_by: "year" %}

{% for g in grouped %}
### {{ g.name }}

<ul>
  {% for t in g.items %}
    <li>
      <strong>{{ t.title }}</strong> —
      {{ t.venue }}
      {% if t.location %}, {{ t.location }}{% endif %}
      {% if t.note %} <em>({{ t.note }})</em>{% endif %}
      {% if t.slides %} · <a href="{{ t.slides }}">Slides</a>{% endif %}
      {% if t.video %} · <a href="{{ t.video }}">Video</a>{% endif %}
    </li>
  {% endfor %}
</ul>
{% endfor %}

{% if site.talks and site.talks.size > 0 %}
---

## Detailed talk pages
{% for post in site.talks reversed %}
  {% include archive-single-talk.html %}
{% endfor %}
{% endif %}
