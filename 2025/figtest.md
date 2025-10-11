---
layout: post
title: "FIG All-Around (WAG) 2025"
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
         {%- assign figScores = site.data.figwagaa2025.scores | where "lc" , "4" -%}
            {%- for score in figScores -%}
             <tr>
               <td class="Country" >{{ score.Fed }}</td>
               <td class="Name" >{{ score.Name }}</td>
               <td class="Total" ><strong>{{ score.Total }}</strong></td>
               <td class="VT" >{{ score.VT }}</td>
               <td class="UB" >{{ score.UB }}</td>
               <td class="BB" >{{ score.BB }}</td>
               <td class="FX" >{{ score.FX }}</td>
               <td class="ND" ><I>{{ score.ND }}</I></td>
               <td class="Event" >{{ score.Event }}</td>
               <td class="Date" >{{ score.Date }}</td>
             </tr>
            {%- endfor -%}
</tbody>
</table>
