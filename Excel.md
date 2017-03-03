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
   <img src="{{ site.baseurl }}/images/1a.png" style="width:450px;">
   <ul>
      <li>Select all cells in the column where the formula or value is to be copied.
          E2 = C2*D2 </li>
   </ul>

   <img src="{{ site.baseurl }}/images/1b.png" style="width:450px;">   
   <ul>
      <li>Press <b>Ctrl + D.</b></li>
   </ul>
   <img src="{{ site.baseurl }}/images/1c.png" style="width:450px;">
   <br>
<hr>
   
   <br>
   <li><b>Filling Empty Excel Rows with Data from the Rows Above</b></li>
   <br>
   <img src="{{ site.baseurl }}/images/2a.jpg" style="width:350px;">
   <ul> 
      <li>Select the column with blank cells. (Product Name column)</li>
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

