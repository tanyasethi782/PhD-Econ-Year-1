# Solutions: 
## Solution 1: Exogenous Selection 

* <u>Assumption</u>: The censoring is random 
* The exact number is the point identification 
* Conditioning on the appropriate X's, one could make a case of exogenous selection but JPepper still thinks its too much of an assumption 
## Solution 2: Worst-Case Bounds 
* (Manski's innovation)
* Also known as Sharp Bounds 
* Width: $P[Z=0| X]$ $\implies$ You need to worry about censoring if this is large i.e. a large proportion of observation are censored  
* Don't confuse with Confidence Intervals 
* This gives us partial identification 
* If the distribution is not Bernoulli $\implies$ replace Law of total probability with LIE 

## Solution 3: Middle Ground Assumptions: 
### 1) IV: 
* $V$ is related to the probability of observation but the outcome is independent of it 
* It is the IV estimator! 

### 2) Heckman Selection Model 
(What is this?)

<u>Reservation Wage Model</u>
Let $Y$ = market wage, $R$ = Reservation Wage (unobserved), 
$Z$ = 1 if $Y \geq$ R; 0, otherwise 

$$log Y = X\beta_2 + \epsilon_1 \\
log R = X\beta_2 + \epsilon_2 \\
P(\epsilon_1,\epsilon_1| X) ~ N(0, \Sigma)
$$

^ Results are very sensitive to the last equation. 



