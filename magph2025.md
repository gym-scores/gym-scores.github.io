---
layout: post
title: "Pommel Horse 2025"
date: 2025-10-07 06:00:00 -0700
discipline: "MAG"
---


<table 
    style="width: 95%;"
     data-pagination="true"
      data-search="true"
    class="table table-striped">
    <tr>
      <th data-sortable="true">Country</th>
      <th data-sortable="true">Name</th>
      <th data-sortable="true">D</th>
      <th data-sortable="true">E</th>
      <th data-sortable="true">ND</th>
      <!-- <th data-sortable="true">Bonus</th> -->
      <th data-sortable="true">Score</th>
      <th data-sortable="true">Event</th>
      <th data-sortable="true">Date</th>  
    </tr>
    {%- for item in site.data.magph2025.scores -%}
    <tr>
      <td class="Country" >{{ item.Fed }}</td>
      <td class="Name" >{{ item.Name }}</td>
      <td class="D" >{{ item.D }}</td>
      <td class="E" >{{ item.E }}</td>
      <td class="ND" >{{ item.ND }}</td>
     <!-- <td class="Bonus" >{{ item.Bonus }}</td> -->
      <td class="Score" >{{ item.Score }}</td>
      <td class="Event" >{{ item.Event }}</td>
      <td class="Date" >{{ item.Date }}</td>
    </tr>
  {%- endfor -%}
</table>
