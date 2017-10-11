---
layout: default
---

# Die Möglichmacher

Die Kosten für das BarCamp werden nur zu einem kleinen Teil durch die Einnahmen aus den [Ticket-Verkäufen]({{ "/Tickets.html" | prepend:site.baseurl }}) gedeckt.

Damit nicht nur die Inhalte stimmen, sondern zum Beispiel auch das Essen und die Getränke freuen wir uns, dass wir 
wieder Sponsoren gewinnen konnten, die das BarCamp Konzept unterstützen.

{% if page.barcamp %}{% assign barcampId = page.barcamp %}{% else %}{% assign barcampId = site.barcamp %}{% endif %}
{% assign barcamp = site.data.barcamps[barcampId] %}
{% for sponsor in barcamp.sponsors %}
 * [{{ sponsor.title }}]({{ sponsor.url }}){% endfor %}s

## Werden Sie Sponsor und unterstützen Sie das BarCamp RheinMain

Das Publikum von BarCamps besteht aus einer interessanten, technisch afinen Gruppe. BarCamps bieten die einmalige Möglichkeit Opinionleader, Multiplikatoren, Blogger und Early Adopters direkt zu erreichen. Eine Reihe von Unternehmen haben diesen Vorteil bereits erkannt. Unter anderem Microsoft, Nokia, Samsung und Jack Wolfskin haben bereits das BarCamp in RheinMain unterstützt.
Entdecken Sie die Möglichkeiten des Sponsoring von realen sozialen Netzwerken für Ihre unternehmensweite Web 2.0 Strategie.

Wenn Sie Sponsor für das BarCamp RheinMain werden wollen, [sprechen Sie uns an]({{ "/Kontakt.html" | prepend:site.baseurl }}).
