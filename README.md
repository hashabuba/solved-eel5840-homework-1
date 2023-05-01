Download Link: https://assignmentchef.com/product/solved-eel5840-homework-1
<br>
<h1>Question 1 –</h1>

Consider the polynomial curve fitting example discussed in class. As discussed, when the model order is <em>too </em>small, the training data is generally <em>underfit </em>and when the model order is <em>too </em>high, the result can <em>overfit </em>the training data. Write a small script of code that mimics our polynomial curve fitting function. The code should generate simulated data from the true function with added zero-mean Gaussian noise (with the true function assumed to be sinc function). The code should also generate a separate validation test data set generated in the same way. Then, after fitting the polynomial to the training data across a range of model orders and evaluated on both the training and testing data, your code should generate a plot similar to the one shown in Figure 1. Also, provide a discussion based on your plot about which model order, <em>M</em>, should be used to avoid over-training.

Figure 1: Figure 1.5 from the Bishop textbook. The y-axis corresponds to the root-meansquare error between the predicted and the true value (on either the training data or test data sets). The x-axis corresponds to the model order.

<h1>Question 2 –</h1>

<strong>Recall:</strong>

Assuming a univariate Gaussian data likelihood given <em>N </em>i.i.d. data points:

)                                                     (1)

and a Gaussian prior distribution on the mean:

)                                                         (2)

with fixed variances (, and), the posterior distribution is given by:

<table width="549">

 <tbody>

  <tr>

   <td width="341"><em>p</em>(<em>µ</em>|<strong>X</strong>) = N(<em>µ</em>|<em>µ<sub>N</sub>,σ<sub>N</sub></em><sup>2 </sup>)where</td>

   <td width="208">(3)</td>

  </tr>

 </tbody>

</table>

(4)

(5)

where <em>µ<sub>ML </sub></em>is the maximum likelihood solution for <em>µ </em>given the <em>N </em>data points.

<ul>

 <li>In or Binomial/Beta example in class, we computed the ML and MAP solutions for the <em>µ </em>parameter of the Binomial distribution iteratively with an increasing number of trials/random draws. Recall, the parameter <em>µ </em>represented the probability of heads.</li>

 <li>In this homework question, you will do the same sort of experiment for random draws from a Gaussian distribution (i.e., a Gaussian data likelihood) with a Gaussian prior distribution on the mean parameter (assume a fixed, known variance for both the Gaussian likelihood and Gaussian prior).</li>

 <li>Write a script that iteratively draws one data point from the true Gaussian distribution (with known mean). Each iteration, compute and ML solution and the MAP solution for the Gaussian mean. After each draw, update the prior distribution to be replaced with the posterior distribution from the previous draw (just like the Binomal/Beta example in class).</li>

 <li>In your solution, provide:</li>

</ul>

<strong>– </strong>Display multiple sample runs of your code and include a description of what the code shows you about ML vs MAP solutions. Your discussion should illustrate that you understand ML and MAP concepts and their differences. Your discussion should answer, at a minimum, the following questions:

∗ What happens when the prior mean is initialized to the wrong value? To the correct value?

∗ What happens as you vary the prior variance from small to large?

∗ What happens when the likelihood variance is varied from small to large?

∗ How do the initial values of the prior mean, prior variance, and likelihood variance interact to effect the final estimate of the mean?

<h1>Question 3</h1>

Consider <em>f</em>(<strong>x</strong>) = 3<strong>x</strong><em><sup>T</sup></em><strong>x </strong>+ 4<strong>y</strong><em><sup>T</sup></em><strong>x </strong>− 1 where <strong>x</strong><em>,</em><strong>y </strong>∈ R<em><sup>d</sup></em>.

<ol>

 <li>What is ? Show your work.</li>

</ol>

<h1>Question 4</h1>

Consider <em>f</em>(<strong>x</strong>) = −10<strong>x</strong><em><sup>T</sup></em><strong>Qx </strong>+ 4<strong>y</strong><em><sup>T</sup></em><strong>x </strong>+ 2 where <strong>x</strong><em>,</em><strong>y </strong>∈ R<em><sup>d</sup></em>, <strong>Q </strong>∈ R<em><sup>d</sup></em><sup>×<em>d </em></sup>and <strong>Q </strong>is symmetric.

<ol>

 <li>What is ? Show your work.</li>

</ol>

<h1>Question 5</h1>

Consider <em>f</em>(<strong>x</strong>) = 8<strong>x</strong><em><sup>T</sup></em><strong>Qx </strong>− 2<strong>y</strong><em><sup>T</sup></em><strong>Q</strong><em><sup>T</sup></em><strong>x </strong>+ 6 where <strong>x</strong><em>,</em><strong>y </strong>∈ R<em><sup>d</sup></em>, <strong>Q </strong>∈ R<em><sup>d</sup></em><sup>×<em>d </em></sup>and <strong>Q </strong>is symmetric.

<ol>

 <li>What is ? Show your work.</li>

 <li>What is ? Show your work.</li>

</ol>

<h1>Question 6</h1>

Consider  where <strong>x </strong>∈ R<em><sup>d</sup></em>.

<ol>

 <li>What is ? Show your work.</li>

</ol>