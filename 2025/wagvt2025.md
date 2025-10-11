---
layout: post
title: "Vault (WAG) 2025"
date: 2025-10-07 06:00:00 -0700
discipline: "WAG"
---

<table id="apparatus"
   class="table table-striped">
<thead>
   <tr>
      <th>Country</th>
      <th>Name</th>
      <th>D 1</th>
      <th>E 1</th>
      <th>ND 2</th>
      <th>Score 1</th>
      <th>D 2</th>
      <th>E 2</th>
      <th>ND 2</th>
      <th>Score 2</th>
      <th>Bonus</th>
      <th>Average</th>
      <th>Combined D</th>
      <th>Event</th>
      <th>Date</th>  
    </tr>
</thead>
      <tbody>
   {%- for item in site.data.wagvt2025.scores -%}
    <tr>
      <td class="Country" >{{ item.Fed }}</td>
      <td class="Name" >{{ item.Name }}</td>
      <td class="D 1" >{{ item.D1 }}</td>
      <td class="E 1" >{{ item.E1 }}</td>
      <td class="ND 1" ><i>{{ item.ND1 }}</i></td>
      <td class="Score 1" ><strong>{{ item.Score1 }}</strong></td>
      <td class="D 2" >{{ item.D2 }}</td>
      <td class="E 2" >{{ item.E2 }}</td>
      <td class="ND 2" ><i>{{ item.ND2 }}</i></td>
      <td class="Score 2" ><strong>{{ item.Score2 }}</strong></td>
      <td class="Bonus">{{ item.Bonus }}</td>
      <td class="Average"><strong><u>{{ item.Average }}</u></strong></td>
      <td class="Combined D">{{ item.CombinedD }}</td>
      <td class="Event" >{{ item.Event }}</td>
      <td class="Date" >{{ item.Date }}</td>
    </tr>
         {%- endfor -%}
</tbody>
</table>

