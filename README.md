Download Link: https://assignmentchef.com/product/solved-assignment-1-cs-750-850-machine-learning
<br>
<span style="font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;">The instructions are geared towards R users. The comments in [P: xxx] are meant as hints to Python users.</span>

Feel free to achieve the results using commands other than the ones mentioned. R, especially, shines when it comes to processing and visualization of structured data, but you would not be able to tell from the ISL book. It uses the oldest and simplest (and ugliest) subset of R. I recommend checking out dplyr for data processing [3,4] and GGPlot [1,4] for plotting.

<h1>Problem 1 [25%]</h1>

In this exercise you will create some simulated data and will fit simple linear regression models to it. Make sure to use set.seed(1) [P: np.random.seed(1)] prior to starting part (1) to ensure consistent results.

<ol>

 <li>Using the rnorm() [P: np.random.normal] function, create a vector, x, containing 100 observations drawn from a<em>√ N</em>(0<em>,</em>3) distribution (Normal distribution with the mean 0 and the <strong>standard deviation</strong></li>

</ol>

3). This represents a feature, <em>X</em>.

<ol start="2">

 <li>Using the rnorm() function, create a vector, eps, containing 100 observations drawn from a<em>√ N</em>(0<em>,</em>0<em>.</em>5)</li>

</ol>

distribution i.e. a normal distribution with mean zero and standard deviation             0<em>.</em>5.

<ol start="3">

 <li>Using x and eps, generate a vector y according to the model <em>Y </em>:</li>

</ol>

<em>Y </em>= <em>−</em>2 + 0<em>.</em>6<em>X </em>


What is the length (number of elements) of y? What are the values of <em>β</em><sub>0</sub><em>,β</em><sub>1 </sub>in the equation above (intercept and slope)?

<ol start="4">

 <li>Create a scatterplot displaying the relationship between x and y. Comment on what you observe. [P: see [2]]</li>

 <li>Fit a least squares linear model to predict y using x. Comment on the model obtained. How do <em>β</em><sup>ˆ</sup><sub>0</sub><em>,β</em><sup>ˆ</sup><sub>1 </sub>compare to <em>β</em><sub>0</sub><em>,β</em><sub>1</sub>?</li>

 <li>Display the least squares line on the scatterplot obtained in 4.</li>

 <li>Now fit a polynomial regression model that predicts <em>y </em>using <em>x </em>and <em>x</em><sup>2</sup>. Is there evidence that the quadratic term improves the model fit? Explain your answer.</li>

</ol>

<h1>Optional Problem O1 [30%]</h1>

This problem can be substituted for Problem 1 above, for up to 5 points extra credit. At most one of the problems 1 and O1 will be considered.

Read Chapter 1 and solve Exercises <em>1.6 </em>and <em>1.10 </em>in [Bishop, C. M. (2006). Pattern Recognition and Machine Learning].

<h1>Problem 2 [25%]</h1>

Read through Section 2.3 in ISL. Load the Auto data set and <em>make sure to remove missing values from the data</em>. Then answer the following questions:

<ol>

 <li>Which predictors are <em>quantitative </em>and which ones are <em>qualitative</em>?</li>

</ol>

1

<ol start="2">

 <li>What is the range, mean, and standard deviation of each predictor? Use range() [pandas.DataFrame.min and max] function.</li>

 <li>Investigate the predictors graphically using plots. Create plots highlighting relationships between predictors. See [1] for a ggplot cheatsheet.</li>

 <li>Compute the matrix of correlations between variables using the function cor() [P: pandas.DataFrame.corr]. Exclude the name variable.</li>

 <li>Use the lm() function to perform a multiple linear regression with mpg as the response. [P: using rpy package is acceptable] Exclude name as a predictor, since it is qualitative. Briefly comment on the output: What is the relationship between the predictors? What does the coefficient for year variable suggest?</li>

 <li>Use the symbols * and : to fit linear regression models with interaction effects. What do you observe?<em>√</em></li>

 <li>Try a few different transformations of variables, such as log(<em>X</em>), <em>X</em>, <em>X</em><sup>2</sup>. What do you observe?</li>

</ol>

<h1>Problem 3 [25%]</h1>

Using equation (3.4) in ISL, argue that in the case of simple linear regression, the least squares line always passes through the point (¯<em>x,y</em>¯).

<h1>Problem 4 [25%]</h1>

It is claimed in the ISL book that in the case of simple linear regression of <em>Y </em>onto <em>X</em>, the <em>R</em><sup>2 </sup>statistic (3.17) is equal to the square of the correlation between <em>X </em>and <em>Y </em>(3.18). Prove that this is the case. For simplicity, you may assume that <em>x</em>¯ = ¯<em>y </em>= 0.

<h1>References</h1>

Each reference is a link. Please open the PDF in a viewer if it is not working on the website.

<ol>

 <li><a href="https://github.com/rstudio/cheatsheets/raw/master/data-visualization-2.1.pdf">R GGPlot cheat sheet</a></li>

 <li><a href="https://machinelearningmastery.com/visualize-machine-learning-data-python-pandas/">Python Pandas data visualization</a></li>

 <li><a href="https://r4ds.had.co.nz/index.html">R For Data Science</a></li>

 <li><a href="https://www.rstudio.com/resources/cheatsheets/">Cheatsheets</a></li>

</ol>

2