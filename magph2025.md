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

<!--<table id="myTable">
    <thead>
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
    </thead>
   <tbody>
    <tr>
      <td class="Country">USA</td>
      <td class="Name">EQUESTRIAN Ryder</td>
      <td class="D">6.0</td>
      <td class="E">9.200</td>
      <td class="ND"></td>
      <td class="Score">15.200</td>
      <td class="Event">Fantasy Camp</td>
      <td class="Date">December 31, 1969</td>
    </tr>
   </tbody>
</table>
-->


<table id="myTable">
<thead>
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
</thead>
   <tbody>
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
   </tbody>
</table>
