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

Michael VK4MWL has pulled together a great guide to DMR hotspots and
how to set yours up.

**Curent File:** [VKDMR Hotspot Setup v1.4.pdf](/assets/dmr/VKDMR Hotspot Setup v1.4.pdf)
{: .notice--info}

## DMR Radio Setup and Etiquette

Bruce VK4EHT has prepared excellent guides on how to configure and use DMR radios.

**Digital voice and etiquette:** [Digital voice net ettiquettev1.0.pdf](/assets/dmr/Digital voice net ettiquettev1.0.pdf)
{: .notice--info}
**DMR talkgroups and timeslots:** [DMR TalkGroups & TimeSlots.pdf](/assets/dmr/DMR TalkGroups & TimeSlots.pdf)
{: .notice--info}
**Configuring a DMR radio:** [General notes for configuring a DMR radio.pdf](/assets/dmr/General notes for configuring a DMR radio.pdf)
{: .notice--info}
**Signal reporting in DMR:** [Signal reporting in DMR.abw.pdf](/assets/dmr/Signal reporting in DMR.abw.pdf)
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

