---
layout: default
title: 3moji - search
---
<!-- Html Elements for Search -->
<div id="search-container">
<input type="text" id="search-input" placeholder="search...">
<ul id="results-container"></ul>
</div>

<!-- Script pointing to search-script.js -->
<script src="js/search-script.js" type="text/javascript"></script>

<!-- Configuration -->
<script>
SimpleJekyllSearch({
  searchInput: document.getElementById('search-input'),
  resultsContainer: document.getElementById('results-container'),
  searchResultTemplate: '<div><a href="{url}"><img width="100px" src="assets/img/3moji/{emoji}.png"/><h2>{title}<h2></a></div>',
  json: '/search.json'
})
</script>