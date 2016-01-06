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
<font face="georgia">
The data for this project is taken from www.dataminingbook.com.

The airlines dataframe used for this project contains 7 variables. All of the 12 variables are integers. The variables are shown in the table below.

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
		<td>Integer/td>
		<td>Number of days since joing the frequent flyer program </td>
	</tr>
</table>
<br>

The dependent variable <i>fiftyKPlus</i> has two classes: *<=50K*  or  *>50K*. Therefore, this being a classification problem, I have developed the following models to predict whether or not a person earns more than 50K annually. I have used R to build the models.

   1. A CART (Classification and Regression Tree) model
   2. A CART model with cross-validation
   3. A Random Forest model
   4. A Logistic Regression model
   

The details of the modelling process and the R code to this project is avaiable <a href = "http://sachinshrestha.github.io/frequentFlyer.html"> here</a>.

To decide which model is best suited to predict whether or not a person earns more than 50K a year, the performance of each model has to be evaluated.


<b>Performance of the models:</b>
<table border="1" style="background-color:#FFFFCC;border-collapse:collapse;border:1px;color:#000000;width:100%" cellpadding="5" cellspacing="3">
	<tr>
		<th>Type of Model</th>
		<th>Baseline Accuracy</th>
		<th>Model Accuracy</th>
		<th>AUC</th>
	</tr>
	<tr>
		<td>CART</td>
		<td></td>
		<td>0.849582</td>
		<td>0.846746</td>
	</tr>
	<tr>
		<td>CART with cross validation</td>
		<td></td>
		<td>0.862403</td>
		<td>0.871933</td>
    </td>
	</tr>
	<tr>
		<td>Random Forest</td>
		<td></td>
		<td>0.825580</td>
		<td>NA</td>
	</tr>
	<tr>
		<td>Logistic Regression</td>
		<td>0.759362</td>
		<td>0.850989</td>
		<td>0.905733</td>
	</tr>
</table>

<br>
Since the accuracy of the *random forest model* is the least of the four models, it may not be best suited for predicting the *label* in this project.

The *logistic regression model* does a little better than the *CART model*. However, the *logistic regression model* is not easily interpretable. Although the model coefficients may be used to determine the significance of *features*, the coefficients do not offer simple explanation of how decision is made. For example, look at the following results for the variable *education* from the summary of the *logistic regression model*.
<section>
<pre><code><font size="2">
occupation Adm-clerical                  -7.306e-02  1.283e-01  -0.569 0.569102
occupation Armed-Forces                  -1.393e+01  9.937e+02  -0.014 0.988812
occupation Craft-repair                   4.995e-02  1.092e-01   0.457 0.647523
occupation Exec-managerial                7.267e-01  1.133e-01   6.414 1.42e-10 ***
occupation Farming-fishing               -1.214e+00  1.851e-01  -6.558 5.46e-11 ***
occupation Handlers-cleaners             -7.398e-01  1.879e-01  -3.938 8.22e-05 ***
occupation Machine-op-inspct             -3.752e-01  1.393e-01  -2.693 0.007089 **
occupation Other-service                 -9.234e-01  1.655e-01  -5.579 2.42e-08 ***
occupation Priv-house-serv               -1.390e+01  2.166e+02  -0.064 0.948837
occupation Prof-specialty                 3.865e-01  1.213e-01   3.186 0.001442 **
occupation Protective-serv                6.512e-01  1.718e-01   3.790 0.000150 ***
occupation Sales                          1.892e-01  1.170e-01   1.617 0.105965
occupation Tech-support                   5.251e-01  1.532e-01   3.428 0.000608 ***
</font></code></pre>
</section>
<br>

Observe how some sub-categories of the variable have been marked as significant (with three asterisks) whereas some are marked as not significant at all. A similar trend can be seen with other variables too. This is complicated! The model is difficult to use to quickly make a prediciton for a new case. In summary, the *logistic regression model* is not easily interpretable.

On the other had, the *CART model* is more easily interpretable. A *CART model* is also preferable because it does not assume a linear model like a *logistic regression model*.

As seen in the plot of the *CART model* (see <a href = "http://sachinshrestha.github.io/census.html"> code</a>), the features that split the tree are *relationship*, *capitalgain* and *education*. The *CART model* is more interpretable in the sense that the model tells that these three features are the strong predictors of whether or not a person earns more than 50K annually.

The *CART model with cross-validation* has the highest accuracy of the models. Although the plot of the *CART model with cross-validation* presents a tree that is more complex than that of the *CART model without cross-validation*, a closer look shows that both the trees have been split by the same three features: *relationship*, *capitalgain* and *education*.

We may thus conclude that, out of the four models, the *CART model with cross-validation* best predicts whether or not a person earns more than $50,000 a year.

And what factors are the strong predictors? Well, as we just saw, the following three factors most signify whether a person earns more than 50K every year:

   1. *relationship*,
   2. *capitalgain* and
   3. *education*.


Here's the complete R code to the<a href = "http://sachinshrestha.github.io/frequentFlyer.html"> Census Project </a>.
</font>

<div id="fb-root"></div>
<script>(function(d, s, id) {
  var js, fjs = d.getElementsByTagName(s)[0];
  if (d.getElementById(id)) return;
  js = d.createElement(s); js.id = id;
  js.src = "//connect.facebook.net/en_US/all.js#xfbml=1";
  fjs.parentNode.insertBefore(js, fjs);
}(document, 'script', 'facebook-jssdk'));</script>

