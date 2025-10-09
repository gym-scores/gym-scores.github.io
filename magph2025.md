---
layout: post
title: "Pommel Horse 2025"
date: 2025-10-07 06:00:00 -0700
discipline: "MAG"
---
   <!-- style="width: 95%;"
     data-pagination="true"
      data-search="true"
    class="table table-striped" --> 

<table id="myTable">
    <tr>
      <th>Country</th>
      <th>Name</th>
      <th>D</th>
      <th>E</th>
      <th>ND</th>
      <th>Score</th>
      <th>Event</th>
      <th>Date</th>  
    </tr>
    <tr>
      <td class="Country" >{{ item.Fed }}</td>
      <td class="Name" >{{ item.Name }}</td>
      <td class="D" >{{ item.D }}</td>
      <td class="E" >{{ item.E }}</td>
      <td class="ND" >{{ item.ND }}</td>
      <td class="Score" >{{ item.Score }}</td>
      <td class="Event" >{{ item.Event }}</td>
      <td class="Date" >{{ item.Date }}</td>
    </tr>
</table>


<!--
<table id="myTable">
    <tr>
      <th>Country</th>
      <th>Name</th>
      <th>D</th>
      <th>E</th>
      <th>ND</th>
      <th>Score</th>
      <th>Event</th>
      <th>Date</th>  
    </tr>
    {%- for item in site.data.magph2025.scores -%}
    <tr>
      <td class="Country" >{{ item.Fed }}</td>
      <td class="Name" >{{ item.Name }}</td>
      <td class="D" >{{ item.D }}</td>
      <td class="E" >{{ item.E }}</td>
      <td class="ND" >{{ item.ND }}</td>
      <td class="Score" >{{ item.Score }}</td>
      <td class="Event" >{{ item.Event }}</td>
      <td class="Date" >{{ item.Date }}</td>
    </tr>
  {%- endfor -%}
</table>
-->
