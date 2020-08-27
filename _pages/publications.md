---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}


{% assign num = 1%}
{% for post in site.publications reversed %}

{% capture foo %}{{ num }}{% endcapture %}
  {% include archive-single.html %}
{% endfor %}