---
layout: post
title: Market Segmentation for Frequent Flyer Program
published: true
date: 2015-11-25
categories: [blogging]
tags: [blogging]
---
<center>![an image alt text]({{ site.baseurl }}/images/frequentFlyer.jpg)</center>

<br>
<br>
<div class="fb-like" data-send="true" data-width="450" data-show-faces="true"></div>
<br>
<br>
<font face="arial">
Market segmentation<sup>1</sup> is a marketing strategy which involves dividing a broad target market into subsets of consumers, businesses, or countries that have, or are perceived to have, common needs, interests, and priorities, and then designing and implementing strategies to target them. Market segmentation strategies are generally used to identify and further define the target customers, and provide supporting data for marketing plan elements such as positioning to achieve certain marketing plan objectives. Businesses may develop product differentiation strategies, or an undifferentiated approach, involving specific products or product lines depending on the specific demand and attributes of the target segment.

In this project, I will analyse the data from an ariline's frequent flyer program. In particular, I will use a <i>clustering algorithm</i> to segment the airline's market into different clusters.

I habe taken the data for this project from www.dataminingbook.com.

The <i>airlines</i> dataframe used for this project contains 7 variables. All of the 12 variables are integers. The variables are shown in the table below.

<table border="1" style="background-color:#FFFFCC;border-collapse:collapse;border:1px;color:#000000;width:100%" cellpadding="5" cellspacing="3">
	<tr>
		<th>Name of Variable</th>
		<th>Variable Type</th>
		<th>Description</th>
	</tr>
	<tr>
		<td>Balance</td>
		<td>Integer</td>
		<td>Frequent flyer points earned so far</td>
	</tr>
	<tr>
		<td>QualMiles</td>
		<td>Integer</td>
		<td>??</td>
	</tr>
	<tr>
		<td>BonusMiles</td>
		<td>Integer</td>
		<td>Miles earned from non-flight transactions</td>
	</tr>
	<tr>
		<td>BonusTrans</td>
		<td>Number of non-flight transactions</td>
	</tr>
	<tr>
		<td>FlightMiles</td>
		<td>Integer</td>
		<td>Miles earned from flight transactions</td>
	</tr>
	<tr>
		<td>FlightTrans</td>
		<td>Integer</td>
		<td>Number of flight transactions</td>
	</tr>
	<tr>
		<td>DaysSinceEnroll</td>
		<td>Integer</td>
		<td>Number of days since joing the frequent flyer program </td>
	</tr>
</table>
<br>

The details of the modelling process and the R code to this project is avaiable <a href = "http://sachinshrestha.github.io/frequentFlyer.html"> here</a>. 

The results from the modelling shows that the airline's customers that are members of its frequent flyer program can be segmented into five distinct clusters. Analysis of each individual cluster shows that the clusters may be described as follows: 

<ol>
<li>Infrequent but loyal customers</li>
<li>Customers with large amout of miles mostly from flight transactions</li>
<li>Customers with large amout of miles mostly from non-flight transactions</li>
<li>New customers accumulating miles from non-fligt transactions</li>
<li>New and infrequent customers</li>  
</ol>


Here's the complete R code to the<a href = "http://sachinshrestha.github.io/frequentFlyer.html"> Market Segmetation for Frequent Flyer Customers Project </a>.
</font>


<h5><sup>1</sup>Wikipedia</h5>

<div id="fb-root"></div>
<script>(function(d, s, id) {
  var js, fjs = d.getElementsByTagName(s)[0];
  if (d.getElementById(id)) return;
  js = d.createElement(s); js.id = id;
  js.src = "//connect.facebook.net/en_US/all.js#xfbml=1";
  fjs.parentNode.insertBefore(js, fjs);
}(document, 'script', 'facebook-jssdk'));</script>

