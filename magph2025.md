---
layout: post
title: "Pommel Horse 2025"
date: 2025-10-07 06:00:00 -0700
discipline: "MAG"
---

<table id="myTable"
   class="table table-striped">
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
      <td class="Score" ><strong>{{ item.Score }}</strong></td>
      <td class="Event" >{{ item.Event }}</td>
      <td class="Date" >{{ item.Date }}</td>
    </tr>
  {%- endfor -%}
   </tbody>
</table>
<script>
   DataTable('#myTable', {
    order: [
        [-3, 'desc'],
        [-5, 'desc'],
         [-6, 'desc']
    ]
});
</script>
