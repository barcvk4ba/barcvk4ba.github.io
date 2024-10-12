---
title: Management Committee
permalink: /docs/management-committee/

# We will define the list of roles and office bearers in
# the _data/office-bearers.yml file so that we can build
# a nice layout below.
#
# it will be available in site.data.officebearers

---

## Management Committee {{ site.data.officebearers.year }}

<table>
    <thead>
        <tr class="header">
            <th>Office</th>
            <th>Bearer</th>
        </tr>
    </thead>
    <tbody>
        {%- for o in site.data.officebearers.offices -%}
        <tr>
            <td><strong>{{ o.office }}</strong></td>
            <td>
                {%- if o.bearer -%}
                    {{ o.bearer }} {%- if o.callsign -%}&nbsp;<small>{{ o.callsign }}</small>{%- endif -%}
                {%- else -%}
                    <small>Vacant</small>
                {%- endif -%}
            </td>
        </tr>
        {%- endfor -%}
    </tbody>
</table>

## Notes
Management Committee positions are elected at the Annual General Meeting which is held in July of each year.

