---
layout: page
permalink: /publications/
title: Artigo Científico
description: "publicações por categorias em ordem cronológica inversa. gerado pelo jekyll-scholar."
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

{% bibliography %}

</div>

<script>
document.addEventListener("DOMContentLoaded", function() {
  var input = document.getElementById("bibsearch");
  if(input) { input.placeholder = "Digite para filtrar..."; }
});
</script>
