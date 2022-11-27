---
layout: single
sidebar:
  nav: repos
title: Repositories
permalink: /repos/
---
{% for repository in site.github.public_repositories %}
  * [{{ repository.name }}]({{ repository.html_url }}) -- {{ repository.description }}
{% endfor %}
