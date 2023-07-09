---
layout: page
title: Search
permalink: /search/
---
<!-- Html Elements for Search -->
<div id="search-container">
<input type="text" id="search-input" placeholder="Type to Search">
<ul id="results-container"></ul>
</div>

<!-- Script pointing to search-script.js -->
<script src="{{ site.baseurl }}/assets/js/search-script.js" type="text/javascript"></script>

<!-- Configuration -->
<script>
SimpleJekyllSearch({
    searchInput: document.getElementById('search-input'),
    resultsContainer: document.getElementById('results-container'),
    searchResultTemplate: '<div style="text-align: left !important;"><a href="{url}"><h3 style="text-align:left !important;">{title}</h3></a><span style="text-align:left !important;">{date}</span></div>',
    json: '{{ site.baseurl }}/search.json'
    });
</script>