---
layout: default
title: Historie
order: 8
slider: true
---

# Vergangene BarCamps

{% for slug in site.data.history %}{% assign camp = site.data.barcamps[slug] %}
{% assign participants = true %}
{% if camp.disableParticipantList == true %}{% assign participants = false %}{% endif %}
 * {{ site.title }} {{ camp.title }}
   * <a href="{{ "/Nachlese-" | prepend: site.baseurl | append:slug | append:".html" }}">Nachlese</a>
   * <a href="{{ "/Location-" | prepend: site.baseurl | append:slug | append:".html" }}">Location</a>
   * <a href="{{ "/Sponsoren-" | prepend: site.baseurl | append:slug | append:".html" }}">Sponsoren</a>{% if participants %}
   * <a href="{{ "/Teilnehmer-" | prepend: site.baseurl | append:slug | append:".html" }}">Teilnehmer</a>{% endif %}
   * <a href="{{ "/Statistiken-" | prepend: site.baseurl | append:slug | append:".html" }}">Statistiken</a>{% endfor %}
