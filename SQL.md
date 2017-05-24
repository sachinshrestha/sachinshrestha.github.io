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
<br>
<li><b>SELECT aggregated and non-aggregated columns from a table</b></li>
<br>
<ul>
<li>Source table: [Staffing]
<br>Note how the same school appears in multiple rows.</li>
<br>
<img src="{{ site.baseurl }}/images/SQL1.png" style="width:379px"> 
<br><br>      
<li>SQL Code:<br>
</li> 
<br>
<img src="{{ site.baseurl }}/images/SQL2.png" style="width:631px;">      
<br><br>
<li>Resulting table: [Total Staffing Entitlement] is aggregated by School Code.</li>      
<br>
<img src="{{ site.baseurl }}/images/SQL3.png" style="width:418px;">
<br><br>
<li>The same result can be obtained by using a shorter query shown below.</li>      
<br>
<img src="{{ site.baseurl }}/images/SQL4.png" style="width:574px;">
<br>
</ul>  
<hr>
<br>
<li><b>Creating Primary and Foreign keys in existing tables</b></li>
<br>
<ul>
<li>Creating a primary key</li>
<img src="{{ site.baseurl }}/images/SQL_PrimaryKey.png" style="width:468px"> 
<br><br>
<li>Creating a foreign key</li>
<img src="{{ site.baseurl }}/images/SQL_ForeignKey.png" style="width:641px"> 
<br>    
<hr>



