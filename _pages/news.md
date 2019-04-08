---
title: "Les derniers ajouts"
layout: single
permalink: /news/
sidebar:
  nav: "navigation"
---
Retrouvez ici les 10 derniers liens, livres & co que j'ai ajoutés.

{% assign links = site.links| slice :0,10 | sort : date %}
{% include links_loop.md %}