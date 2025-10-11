---
layout: post
title: "FIG-only All-Around (WAG) 2025"
date: 2025-10-07 06:00:00 -0700
discipline: "WAG"
---

<table id="apparatus"
   class="table table-striped">
<thead>
   <tr>
      <th>Country</th>
      <th>Name</th>
      <th>Total</th>
      <th>VT</th>
      <th>UB</th>
      <th>BB</th>
      <th>FX</th>
      <th>ND</th>
      <th>Event</th>
      <th>Date</th>  
    </tr>
</thead>
      <tbody>
        {%- if site.data.figwagaa2025.scores.lc < 5 -%}
         {%- for item in site.data.figwagaa2025.scores -%}
    <tr>
      <td class="Country" >{{ item.Fed }}</td>
      <td class="Name" >{{ item.Name }}</td>
      <td class="Total" ><strong>{{ item.Total }}</strong></td>
      <td class="VT" >{{ item.VT }}</td>
      <td class="UB" >{{ item.UB }}</td>
      <td class="BB" >{{ item.BB }}</td>
      <td class="FX" >{{ item.FX }}</td>
      <td class="ND" ><I>{{ item.ND }}</I></td>
      <td class="Event" >{{ item.Event }}</td>
      <td class="Date" >{{ item.Date }}</td>
    </tr>
          {%- endfor -%}
         {%- endif -%}
</tbody>
</table>

