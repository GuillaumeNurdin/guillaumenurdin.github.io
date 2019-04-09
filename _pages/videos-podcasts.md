---
title: Les vidéos et podcasts
layout: single
type: video
toc: true
toc_label: "Dans cette page"
toc_icon: "cog"
sidebar:
  nav: "navigation"
permalink : /videos-podcasts/
---
{% include page_icon.md%}/<i class="{{site.data.types['podcast'].fa}}" aria-hidden="true"></i>
On trouve de très bonnes vidéos (souvent filmées lors de conférence ou de meetup) et podcasts en français. J'aime bien profiter de temps à autres des transports pour les écouter. Vous retrouverez ici aussi quelques vidéos immanquables en anglais.
{: .notice--info}
{% assign groupby = "category" %}
## Les vidéos
{% assign links_filtered = site.links | where:"type", 'video' %}
{% include links_collection_groupby.md %}

## les podcasts
{% assign links_filtered = site.links | where:"type", 'podcast' %}
{% include links_collection_groupby.md %}