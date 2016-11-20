---
layout: default
title: Historie
order: 8
slider: true
---

# Vergangene BarCamps

{% for slug in site.data.history %}{% assign camp = site.data.barcamps[slug] %}
 * {{ site.title }} {{ camp.title }}
   * <a href="{{ "/Location-" | prepend: site.baseurl | append:slug | append:".html" }}">Location</a>
   * <a href="{{ "/Sponsoren-" | prepend: site.baseurl | append:slug | append:".html" }}">Sponsoren</a>
   * <a href="{{ "/Teilnehmer-" | prepend: site.baseurl | append:slug | append:".html" }}">Teilnehmer</a>
   * <a href="{{ "/Statistiken-" | prepend: site.baseurl | append:slug | append:".html" }}">Statistiken</a>{% endfor %}
