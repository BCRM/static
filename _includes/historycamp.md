{% assign camp = site.data.barcamps[page.barcamp] %}
{% assign participants = true %}
{% if camp.disableParticipantList == true %}{% assign participants = false %}{% endif %}
{% assign statistics = true %}
{% if camp.disableStatistics == true %}{% assign statistics = false %}{% endif %}

# {{ site.title }} {{ camp.title }}

* <a href="{{ "/Nachlese-" | prepend: site.baseurl | append:slug | append:".html" }}">Nachlese</a>
* <a href="{{ "/Location-" | prepend: site.baseurl | append:slug | append:".html" }}">Location</a>
* <a href="{{ "/Sponsoren-" | prepend: site.baseurl | append:slug | append:".html" }}">Sponsoren</a>{% if participants %}
* <a href="{{ "/Teilnehmer-" | prepend: site.baseurl | append:slug | append:".html" }}">Teilnehmer</a>{% endif %}{% if statistics %}
* <a href="{{ "/Statistiken-" | prepend: site.baseurl | append:slug | append:".html" }}">Statistiken</a>{% endif %}
