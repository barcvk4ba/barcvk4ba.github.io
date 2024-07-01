---
title: DMR Information
permalink: /articles/dmr/
toc: true
read_time: false
author_profile: false
#
# This page is designed to collect articles that are tagged as 'dmr'
# If you create an article in the _articles folder and add front matter of
#   tags: dmr
# it will appear in this page/list
#
---
## VKDMR Hotspot Setup

Michael Lanagan (VK4MWL) has pulled together a great guide to DMR hotspots and
how to set yours up.

**Curent File:** [VKDMR_Hotspot_Setup_v1.3.pdf](/assets/dmr/VKDMR_Hotspot_Setup_v1.3.pdf)
{: .notice--info}

## Links

* Repeaters [http://rpt.vkdmr.com/](http://rpt.vkdmr.com/){:target="_blank"}
* Hot Spots [http://hot.vkdmr.com/](http://hot.vkdmr.com/){:target="_blank"}
* VK DMR [https://vkdmr.com/](https://vkdmr.com/){:target="_blank"}

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

It's your hobby so get active and turn your radio on
