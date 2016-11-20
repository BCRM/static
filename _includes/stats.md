## Statistiken

{% if page.barcamp %}{% assign barcampId = page.barcamp %}{% else %}{% assign barcampId = site.barcamp %}{% endif %}

<div id="stats" data-barcampid="{{ barcampId }}"></div>
<script type="text/javascript" src="{{ "/js/mustache.js" | prepend: site.baseurl }}"></script>
<script type="text/javascript" src="{{ "/js/stats.js" | prepend: site.baseurl }}"></script>
<script type="text/javascript" src="//www.google.com/jsapi"></script>
<script type="text/javascript">
    google.load("visualization", "1", {packages: ["corechart"]});
    google.setOnLoadCallback(function () {
        Stats($('#stats'));
    });
</script>
