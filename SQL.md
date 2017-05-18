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
      <br>      
      <li>SQL Code: Two separate SELECT statements are used to create two tables that are then JOINed in a third (outer) SELECT statement</li> 
      <br>
      <img src="{{ site.baseurl }}/images/SQL2.png" style="width:450px;">      
      <br>
      <li>Resulting table:</li>      
      <br>
      <img src="{{ site.baseurl }}/images/SQL3.png" style="width:450px;">
      <br>
   </ul>      
   First, to select the column with blank cells. (Product Name column)
   <ul>     
      <li>Click <b>Find and Select</b>.</li> 
      <li>Choose <b>Go To Special…</b>.</li>
   </ul>
   <br>
   <img src="{{ site.baseurl }}/images/2b.jpg" style="width:200px;"> 
   <ul>
      <li>Choose <b>Blanks</b> and OK that.</li>
   </ul>
    <br>
   <img src="{{ site.baseurl }}/images/2c.jpg" style="width:280px;">
  <br>
  <br>
  <ul>
      <li>Now push the <b>Equals (=)</b> key, then the <b>Up Arrow</b> and finally, <b>Ctrl + Enter</b>.</li>
   </ul>
   <br>
   <img src="{{ site.baseurl }}/images/2d.jpg" style="width:350px;">
   <br>
   
   <hr>
   <br>
   <li><b>INDEX() and MATCH()</b></li>
   <br>
Problem: Import values for <b>Price</b> column in <b>Table 1</b> from <b>Price</b> column in <b>Table 2</b> using <b>Product ID</b> as intersecting key.
   <br>
   <img src="{{ site.baseurl }}/images/3a.png" style="width:500px;">
   <br>
   
   
   <ul> 
      <li>Start with MATCH(): Match <b>Product ID</b> value in <b>Table 1</b> with <b>Product ID</b> column in <b>Table 2</b>.</li>
      <img src="{{ site.baseurl }}/images/3b.png" style="width:200px;">
   </ul>
   <br>
   
   
   <ul>
      <li>Follow with INDEX(): Index the <b>Price</b> column in <b>Table 2</b>.</li>
      <img src="{{ site.baseurl }}/images/3c.png" style="width:300px;">
   </ul>

   
   <br>
   <ul>
      <li>Final table below.</li>
      <img src="{{ site.baseurl }}/images/3d.png" style="width:300px;">     
   </ul>
   </ol>

