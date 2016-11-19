---
layout: default
---

# Teilnehmerliste

{% for participant in site.data.participants %}
 * {% if participant.twitter %}<a href="https://twitter.com/{{ participant.twitter }}">{% endif %}{{ participant.name }}{% if participant.twitter %}</a>{% endif %} {% if participant.tags %}<small>// {{ participant.tags }}</small>{% endif %}{% endfor %}
