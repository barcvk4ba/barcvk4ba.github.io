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

## Links

* Repeaters [http://rpt.vkdmr.com/](http://rpt.vkdmr.com/){:target="_blank"}
* Hot Spots [http://hot.vkdmr.com/](http://hot.vkdmr.com/){:target="_blank"}
* [VK4DRM Repeater Map](https://www.google.com/maps/d/viewer?mid=1pN0ls-uQ6GIixGanunLe0HETqo8&ll=-27.331080754756925%2C153.09384449189344&z=9){:target="_blank"}

## DMR Articles

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

