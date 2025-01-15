---
layout: single
sidebar:
  nav: repos
title: Repositories
permalink: /repos/
---

(Auto generated list of my public repositories)
{% assign non_forked_repos = site.github.public_repositories | where_exp: "item", "item.fork == false" %}
| Repo | Description |
| ---- | ---- |
{% for repository in non_forked_repos -%}
| [{{ repository.name }}]({{ repository.html_url }}) | {{ repository.description | default: "*<font color='gray'>No description...</font>*" }} |
{% endfor %}


