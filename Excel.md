---
title: Excel Tips and Tricks
permalink: /Excel/
layout: page
sitemap: false
---
   <br>
   <ol>
   <li><b>Copying Formulas from Rows above to Rows below in Excel</b></li>
   <br>
   <center><img src="{{ site.baseurl }}/images/1a.jpg" style="width:450px;"></center>       
   <ul>
      <li>Select all cells in the column where the formula or value is to be copied.
          E2 = C2*D2 </li>
   </ul>

   <center><img src="{{ site.baseurl }}/images/1b.jpg" style="width:450px;"></center>       
   <ul>
      <li>Press <b>Ctrl + D.</b></li>
   </ul>
   <center><img src="{{ site.baseurl }}/images/1c.jpg" style="width:450px;"></center>       
   <br>
<hr>
   <br>
   <li><b>Filling Empty Excel Rows with Data from the Rows Above</b></li>
   <br>
   <center><img src="{{ site.baseurl }}/images/2a.jpg" style="width:400px;"></center>       
   <ul> 
      <li>Select the column with blank cells. (Product Name column)</li>
      <li>Click <b>Find and Select</b>.</li> 
      <li>Choose <b>Go To Special…</b>.</li>
   </ul>
   <br>
   <center> <img src="{{ site.baseurl }}/images/2b.jpg" style="width:200px;"> </center> 
   <ul>
      <li>Choose <b>Blanks</b> and OK that.</li>
   </ul>
    <br>
   <center><img src="{{ site.baseurl }}/images/2c.jpg" style="width:300px;"></center>       
   <ul>
      <li>Now push the <b>Equals (=)</b> key, then the <b>Up Arrow</b> and finally, <b>Ctrl + Enter</b>.</li>
   </ul>
   <br>
   <center><img src="{{ site.baseurl }}/images/2d.jpg" style="width:400px;"></center>       
   <br>
   
   <hr>
   <br>
   <li><b>INDEX() and MATCH()</b></li>
   <br>
   Problem: Import values for RAM column in Table 1 from RAM column in Table 2 using School Code as intersecting key.
   <br>
   <center><img src="{{ site.baseurl }}/images/3a.jpg" style="width:350px;">       
   <img src="{{ site.baseurl }}/images/3b.jpg" style="width:200px;"></center>       
   <ul> 
      <li>Start with MATCH(): Match School Code value in Table 1 with School Code column in Table 2.</li>
   </ul>
   <br>
   <center> <img src="{{ site.baseurl }}/images/3c.jpg" style="width:200px;"> </center> 
   <ul>
      <li>2.	Follow with INDEX(): Index the RAM column in Table 2.</li>
   </ul>
       <br>
   <center><img src="{{ site.baseurl }}/images/3d.jpg" style="width:300px;"></center>     
   </ol>

