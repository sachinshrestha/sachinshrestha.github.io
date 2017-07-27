---
layout: post
title: Market Segmentation for Frequent Flyer Program
published: true
date: 2015-11-25
categories: [blogging]
tags: [blogging]
---
![Frequent Flyer]({{ site.url }}/images/frequentFlyer.jpg)

<br>
<br>

Market segmentation<sup>1</sup> is a marketing strategy which involves dividing a broad target market into subsets of consumers, businesses, or countries that have, or are perceived to have, common needs, interests, and priorities, and then designing and implementing strategies to target them. Market segmentation strategies are generally used to identify and further define the target customers, and provide supporting data for marketing plan elements such as positioning to achieve certain marketing plan objectives. Businesses may develop product differentiation strategies, or an undifferentiated approach, involving specific products or product lines depending on the specific demand and attributes of the target segment.

In this project, I will analyse data from an ariline's frequent flyer program to group it's customers into different market segments. In particular, I will use <i>clustering algorithm</i> to segment the airline's market into different clusters.

The data is sourced from  <i>www.dataminingbook.com</i>.

The <i>airlines</i> dataframe contains 7 variables all of which are integers. The variables and their description are shown in the following table.

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
		<td>Number of qualifying miles</td>
	</tr>
	<tr>
		<td>BonusMiles</td>
		<td>Integer</td>
		<td>Miles earned from non-flight transactions</td>
	</tr>
	<tr>
		<td>BonusTrans</td>
		<td>Integer</td>
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

The details of the modelling process and the R code to this project is avaiable <a href = "http://sachinshrestha.github.io/frequentFlyerCode/"> here</a>. 

Results from the model shows that the airline's customers (that are members of its frequent flyer program) can be categorised into five distinct groups. Analysis of each individual group shows that the groups may be broadly described as follows: 

<ol>
<li>Infrequent but loyal customers</li>
<li>Customers with large amount of miles mostly from flight transactions</li>
<li>Customers with large amount of miles mostly from non-flight transactions</li>
<li>New customers accumulating miles from non-flight transactions</li>
<li>New and infrequent customers</li>  
</ol>

Here's the complete R code to the<a href = "http://sachinshrestha.github.io/frequentFlyerCode/"> Market Segmentation for Frequent Flyer Customers Project</a>.
<hr>
<sup>1</sup>Wikipedia


<div class='tableauPlaceholder' id='viz1501130977018' style='position: relative'><noscript><a href='#'><img alt='Dashboard 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;LP&#47;LPPsandtheirSPEs&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='site_root' value='' /><param name='name' value='LPPsandtheirSPEs&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;LP&#47;LPPsandtheirSPEs&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /></object></div>                <script type='text/javascript'>                    var divElement = document.getElementById('viz1501130977018');                    var vizElement = divElement.getElementsByTagName('object')[0];                    vizElement.style.width='1004px';vizElement.style.height='869px';                    var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>
