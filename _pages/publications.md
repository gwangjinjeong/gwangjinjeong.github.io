---
title: "Publications"
permalink: /publications/
layout: archive
author_profile: true
taxonomy: publication
---
# publicated paper

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}