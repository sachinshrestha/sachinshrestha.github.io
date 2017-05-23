---
title: SQL Tips and Tricks
permalink: /SQL/
layout: page
sitemap: false
---
   <br>
   <ol>
   <li><b>SELECT multiple columns in a GROUP BY (aggregation) statement</b></li>
   <br>
   <ul>
      <li>Source table: Note how the same school appears in multiple rows.</li>
      <br>
      <img src="{{ site.baseurl }}/images/SQL1.png" style="width:600px;"> 
      <br><br>      
      <li>SQL Code: Two separate SELECT statements are used to create two tables - one with the required columns ([School Code], [School Name], [Zone]) and the other with the aggregated column (sum([Actual Entitlement]) as TotalFTE). The two tables are then JOINed and required columns ([School Code], [School Name], [Zone], [TotalFTE]) are SELECTed from the outer SELECT statement.</li> 
      <br>
      <img src="{{ site.baseurl }}/images/SQL2.png" style="width:450px;">      
      <br><br>
      <li>Resulting table: TotalFTE is aggregated by School Code.</li>      
      <br>
      <img src="{{ site.baseurl }}/images/SQL3.png" style="width:450px;">
      <br>
   </ul>      
   </ol>
   
