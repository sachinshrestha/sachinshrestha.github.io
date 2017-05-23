---
title: SQL Tips and Tricks
permalink: /SQL/
layout: page
sitemap: false
---
   <br>
   Here's the Database Diagram for the SQL Exercises.
   <br>
   <img src="{{ site.baseurl }}/images/DatabaseDiagram.png" style="width:836px"> 
   <br><br>
   <ol>
   <hr>
   <li><b>SELECT aggregated and non-aggregated columns from a table</b></li>
   <br>
   <ul>
      <li>Source table: Note how the same school appears in multiple rows.</li>
      <br>
      <img src="{{ site.baseurl }}/images/SQL1.png" style="width:604px"> 
      <br><br>      
      <li>SQL Code:<br>
Fist create two tables using two separate SELECT statements. <br> 
Use the first SELECT statement to create a table with the join column and all non-aggregated columns.<br>
Then use the second SELECT statement to create a table with the join column and the aggregated columns.<br>
Finally, use a third SELECT statement to pick the required columns from the joined table.<br>
</li> 
      <br>
      <img src="{{ site.baseurl }}/images/SQL2.png" style="width:424px;">      
      <br><br>
      <li>Resulting table: TotalFTE is aggregated by School Code.</li>      
      <br>
      <img src="{{ site.baseurl }}/images/SQL3.png" style="width:320px;">
      <br>
   </ul>   
   <hr>
   </ol>
   

