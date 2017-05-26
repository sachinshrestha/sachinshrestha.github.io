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

<img src="{{ site.baseurl }}/images/SQL_SyntaxOfSelectStatement.png" style="width:531px"> 
<br><br>
<ol>
<hr>

<li><b>SELECT aggregated and non-aggregated columns from a table</b></li>
<br>
<ul>
<li>Task: List the total Staffing Entitlements for each school.</li>
<br>
<li>Source table: [Staffing]
<br>Note how the same school appears in multiple rows.</li>
<br>
<img src="{{ site.baseurl }}/images/SQL1.png" style="width:379px"> 
<br><br>      
<li>SQL:
</li> 
<br>
<img src="{{ site.baseurl }}/images/SQL2.png" style="width:566px;">      
<br><br>
<li>Result: [Total Staffing Entitlement] is aggregated by School Code.</li>      
<br>
<img src="{{ site.baseurl }}/images/SQL3.png" style="width:418px;">
<br><br>
<li>Alternative: The same result can be obtained by using a shorter query shown below.</li>      
<br>
<img src="{{ site.baseurl }}/images/SQL4.png" style="width:574px;">
<br>
</ul>  
<hr>


<li><b>Creating Primary and Foreign keys in existing tables</b></li>
<br>
<ul>
<li>Creating a primary key</li>
<img src="{{ site.baseurl }}/images/SQL_PrimaryKey.png" style="width:468px"> 
<br><br>
<li>Creating a foreign key</li>
<img src="{{ site.baseurl }}/images/SQL_ForeignKey.png" style="width:595px"> 
<br>
</ul>
<hr>


<li><b>How to SELECT column names in a table</b></li>
<br>
<ul>
<li>SQL:<br>
<img src="{{ site.baseurl }}/images/SQL_ColumnNames.png" style="width:405px"> 
</li>
<br>  
<li>Result:</li>
<img src="{{ site.baseurl }}/images/SQL_ColumnNamesResult.png" style="width:109px"> 
</ul>
<hr>


<li><b>ORDER BY vs HAVING</b></li>
<br>
<ul>
<li>SQL:<br>
<img src="{{ site.baseurl }}/images/SQL_OrderBy_vs_Having.png" style="width:556px"> 
</li>
<br>  
<li>Result:</li>
<br>
<img src="{{ site.baseurl }}/images/SQL_OrderBy_vs_Having_Results.png" style="width:397px"> 
</ul>
<hr>

<li><b>SUBQUERIES</b></li>
<br>
<img src="{{ site.baseurl }}/images/SQL_Subqeries.png" style="width:541px"> 
<ul>
<li>SQL:<br>
<img src="{{ site.baseurl }}/images/SQL_Subqeries_AvgMinMax1.png" style="width:574px"> 
<img src="{{ site.baseurl }}/images/SQL_Subqeries_AvgMinMax2.png" style="width:562px"> 
</li>
<br>  
<li>Result:</li>
<img src="{{ site.baseurl }}/images/SQL_Subqeries_GreaterThanAverageResult.png" style="width:385px"> 
<br>
<img src="{{ site.baseurl }}/images/SQL_Subqeries_MaxMinResult.png" style="width:411px"> 
<br>  

<li>SQL:<br>
<img src="{{ site.baseurl }}/images/SQL_Subqeries_NotPresentInAnotherTable.png" style="width:507px"> 
</li>
<br>  
<li>Result:</li>
<img src="{{ site.baseurl }}/images/SQL_Subqeries_NotPresentInAnotherTableResult.png" style="width:365px"> 
<br>
</ul>
<hr>

