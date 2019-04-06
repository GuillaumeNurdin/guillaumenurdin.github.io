---
title: Les vidéos et podcasts
layout: single
toc: true
toc_label: "Dans cette page"
toc_icon: "cog"
sidebar:
  nav: "navigation"
permalink : /videos-podcasts/
---
{% assign groupby = "category" %}
## Les vidéos
{% assign links_filtered = site.links | where:"type", 'video' %}
{% include links_collection_groupby.md %}

## les podcasts
{% assign links_filtered = site.links | where:"type", 'podcast' %}
{% include links_collection_groupby.md %}