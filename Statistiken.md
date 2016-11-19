---
layout: default
---

## Statistiken

<div id="stats"></div>
<script type="text/javascript" src="/vendor/mustache/mustache.js"></script>
<script type="text/javascript" src="/js/stats.js"></script>
<script type="text/javascript" src="https://www.google.com/jsapi"></script>
<script type="text/javascript">
    google.load("visualization", "1", {packages: ["corechart"]});
    google.setOnLoadCallback(function () {
        Stats($('#stats'));
    });
</script>
