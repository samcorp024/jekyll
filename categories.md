---
layout: default
permalink: /categories/
---

<h1>Categories</h1>

<div class="categories-container">
  {% for category in site.categories %}
    {% assign category_name = category[0] | slugify %}
    <div class="category-card">
      <img src="{{ site.data.categories[category_name].image }}" alt="{{ category[0] | capitalize }} category image">
      <h2><a href="/categories/{{ category_name }}/">{{ category[0] | capitalize }}</a></h2>
      <p>{{ site.data.categories[category_name].description }}</p>
    </div>
  {% endfor %}
</div>

<script>
  document.addEventListener("DOMContentLoaded", function() {
    var baseurl = "";
    if (window.location.pathname === "/") {
      baseurl = "/jekyll";
    }

    // Update href attributes of category links to include baseurl
    var categoryLinks = document.querySelectorAll(".category-card a");
    categoryLinks.forEach(function(link) {
      var href = link.getAttribute("href");
      if (href && !href.startsWith("http")) {
        link.setAttribute("href", baseurl + href);
      }
    });
  });
</script>
