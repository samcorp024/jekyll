---
layout: home
paginate: true
title: Home
---
---
layout: home
paginate: true
title: Home
---

<script>
  // JavaScript to adjust baseurl based on the current path
  document.addEventListener("DOMContentLoaded", function() {
    var baseurl = "";
    if (window.location.pathname === "/") {
      // Check for specific path and set baseurl if needed
      baseurl = "/jekyll";
    }

    // Update href attributes of links to include baseurl
    var links = document.querySelectorAll("a");
    links.forEach(function(link) {
      var href = link.getAttribute("href");
      if (href && !href.startsWith("http")) {
        link.setAttribute("href", baseurl + href);
      }
    });

    // Optionally adjust other elements or data as needed
  });
</script>

<div class="button-container">
  <a href="/categories" class="button">Category</a>
  <a href="/tags/?tag=trending" class="button">Tags</a>
  <a href="/posts" class="button">Posts</a>
</div>

<!-- ## Welcome to My Jekyll Site -->

<!-- This is the main page of my Jekyll site. Explore the different sections using the buttons above.

### Featured Content
- **Latest Post**: [Title of Latest Post](/posts/latest-post-url)
- **Popular Category**: [Popular Category Name](/category/popular-category-url)
- **External Resources**: [Useful Links](/links) -->

<!-- ## Welcome to My Jekyll Site -->

<!-- This is the main page of my Jekyll site. Explore the different sections using the buttons above.

### Featured Content
- **Latest Post**: [Title of Latest Post](/posts/latest-post-url)
- **Popular Category**: [Popular Category Name](/category/popular-category-url)
- **External Resources**: [Useful Links](/links) -->
