---
layout: default
---

## Statistiken

<div id="stats"></div>
<script type="text/javascript" src="{{ "/js/mustache.js" | prepend: site.baseurl }}"></script>
<script type="text/javascript" src="{{ "/js/stats.js" | prepend: site.baseurl }}"></script>
<script type="text/javascript" src="//www.google.com/jsapi"></script>
<script type="text/javascript">
    google.load("visualization", "1", {packages: ["corechart"]});
    google.setOnLoadCallback(function () {
        Stats($('#stats'));
    });
</script>
