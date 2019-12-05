---
title: "Publications"
layout: category
permalink: /publications/
author_profile: true
taxonomy: publication
---

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}