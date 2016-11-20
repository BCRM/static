# Teilnehmerliste

{% if page.barcamp %}{% assign barcampId = page.barcamp %}{% else %}{% assign barcampId = site.barcamp %}{% endif %}
{% assign participants = site.data.participants[barcampId] %}

{% for participant in participants %}
 * {% if participant.twitter %}<a href="https://twitter.com/{{ participant.twitter }}">{% endif %}{{ participant.name }}{% if participant.twitter %}</a>{% endif %} {% if participant.tags %}<small>// {{ participant.tags }}</small>{% endif %}{% endfor %}
