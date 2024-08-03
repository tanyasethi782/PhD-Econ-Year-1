


# Single Hypothesis Testing 
<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
* $\frac{b_n - \beta}{\sigma}$ < critical value 
* Notice it is $\sigma$ and NOT $\sigma^2$
* follows Z distribution 


# Joint Hypothesis Testing 
<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

* Wald Test (Without Matrices): 
$W = \frac{(y- \mu)^2}{\Sigma}$

$\Sigma =$ variance

* Wald Estimator (With Matrices): 
(how we did in class): 
$w = (Hb_n - H\beta)'(H\Sigma H)^{-1}(Hb_n - H\beta)$ < critical value 
Wald Estimator follows Chi square distribution 
* $\Sigma= \frac{e'e}{n-k}(X'X)^{-1}$, when $\sigma$ is unknown
* $\Sigma= \sigma(X'X)^{-1}$, when $\sigma$ is known





* Joint Confidence Region 
$w = (Hb_n - H\beta)'(H\Sigma H)^{-1}(Hb_n - H\beta)$ < critical value 

(except leave beta as it is)
Also \beta = {B1
			B2}
		Long matrix 

* Wald Estimator in terms of R^2 : 

$W = (N-K)(R^2 - R^{2*})/(1-R^2)$, where $R^2$ : corresponds to long regression \& $R^{2*}$ corresponds to short regression

Also,  $W = (N-k)(e*'e* - e'e)/(1-e'e)$

Note:  $R^2 = e'e$' 
$e'e = S^{2}(N-k)$


# Power of the test 
<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

* Calculate power of the test at critical value -1.645 for both sides and when $\beta = -2$ 
$P (z< -1.645 | \beta = -2) + P (z> -1.645 | \beta = -2)$
$P (z< -1.645 - (-2)) + P (z> -1.645 - (-2))$
$P (z< 0.36) + P (z> 2.645)$
^ Check these values from the z-tables 

* We also consider the variance. There is more that goes in the construction of z which I have not explained here. 