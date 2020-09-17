---
title: DMR Information
permalink: /articles/dmr/
toc: false
read_time: false
author_profile: false
#
# This page is designed to collect articles that are tagged as 'dmr'
# If you create an article in the _articles folder and add front matter of
#   tags: dmr
# it will appear in this page/list
#
---

A collection of articles related to DMR

{%
assign entries = site.articles
        | where_exp: "item", "item.tags contains 'dmr'"
        | sort: 'date'
        | reverse %}

{%- for post in entries -%}
  {%- unless post.hidden -%}
    {% include archive-single.html %}
  {%- endunless -%}
{%- endfor -%}

