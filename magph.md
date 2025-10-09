---
layout: post
title: "Pommel Horse"
date: 2025-08-07 06:00:00 -0700
discipline: "MAG"
---

{%- for item in site.data.magph.scores -%}
    <p>{{ item.Fed }}</p>
{%- endfor -%}

<!-- <table style="width: 95%;">
    <tr>
      <th>Country</th>
      <th>Name</th>
      <th>D</th>
      <th>E</th>
      <th>ND</th>
      <th>Bonus</th>
      <th>Score</th>
      <th>Event</th>
      <th>Date</th>
    </tr>
    <tr>
      <td>
          {%- for item in site.data.magph.scores -%}
              {{ item.Fed }}
          {%- endfor -%}
      </td>
      <td>
          {%- for item in site.data.magph.scores -%}
              {{ item.Name }}
          {%- endfor -%}
        </td>
      <td>
          {%- for item in site.data.magph.scores -%}
              {{ item.D }}
          {%- endfor -%}    
      </td>
      <td>
          {%- for item in site.data.magph.scores -%}
              {{ item.E }}
          {%- endfor -%}</td>
      <td>
          {%- for item in site.data.magph.scores -%}
              {{ item.ND }}
          {%- endfor -%}</td>
      <td>
          {%- for item in site.data.magph.scores -%}
              {{ item.Bonus }}
          {%- endfor -%}</td>
      <td>
          {%- for item in site.data.magph.scores -%}
              {{ item.Score }}
          {%- endfor -%}</td>
      <td>
          {%- for item in site.data.magph.scores -%}
              {{ item.Event }}
          {%- endfor -%}</td>
      <td>
          {%- for item in site.data.magph.scores -%}
              {{ item.Date }}
          {%- endfor -%}</td>
    </tr>
</table>
-->
