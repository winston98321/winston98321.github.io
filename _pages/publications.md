---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

{% assign sorted_pubs = site.publications | sort: 'date' | reverse %}
{% assign current_year = "" %}
{% for post in sorted_pubs %}
  {% assign pub_year = post.date | date: "%Y" %}
  {% if pub_year != current_year %}
    {% assign current_year = pub_year %}
## {{ pub_year }}
  {% endif %}
  {% include archive-single.html %}
{% endfor %}
