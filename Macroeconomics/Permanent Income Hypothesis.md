Robert Hall was the first to derive the effects of rational expectations for consumption. His theory states that if Milton Friedman’s [permanent income hypothesis](https://en.wikipedia.org/wiki/Permanent_income_hypothesis "Permanent income hypothesis") is correct, which in short says current income should be viewed as the sum of permanent income and transitory income and that consumption depends primarily on permanent income, and if consumers have rational expectations, then any changes in consumption should be unpredictable, i.e. follow a random walk.



* Bliss Point: Quantity of consumption where any further increase would make the consumer less satisfied. It is a quantity of consumption which maximizes utility in the absence of budget constraint.



Random Walk of Consumption: 

(https://web.stanford.edu/~rehall/Stochastic-JPE-Dec-1978.pdf)
![[Pasted image 20240131111204.png]]

Notes: 

# Consumption Smoothing Theory

## <span class = "teal-text">Why do consumers want a way to smooth their consumption?</span>
- Concavity of preference;  Diminishing marginal utility 
- The theory is powerful because it is centrally based on this assumption. It's a widely accepted simple assumption of donor behaviour.
* <span class="dark-mustard-text"> How is this related? Remember, there are other theories too that follow because of concavity</span>
* 
## Partial Equilibrium 

Rep HH chooses Ct, Bt, At to maximize:
$$E_0 \sum_{t=0}^\infty \beta^t \ln(C_t)$$
conditional on all info at period 0

Subject to:
$$C_t + \frac{B_t}{P_t} + A_t = Y_t - T_t+ \frac{(1+i_{t-1})B_{t-1}}{P_t} + (1+r_{t-1})A_{t-1} \quad \forall t$$
$Y_t$ exog
HHs take as given $P_t$, $i_t$, $r_t$, $T_t$, $Y_t$

<span class ="dark-mustard-text" >
Lagrangian:</span>
$$L = E_0  \sum_{t=0}^\infty \beta^t \left[\ln(C_t) + \lambda_t (Y_t -T_t + \frac{(1+i_{t-1})B_{t-1}}{P_t} + (1+r_t)A_{t-1} - C_t - \frac{B_t}{P_t} - A_t) \right]$$


Just to clarify: $\lambda_t$ is the shadow value of relaxing the budget constraint by a unit. When you relax the constraint, you increase the consumption. 



# Consumer's Decision

If prices are sticky, at time $t$, the consumer is deciding:

$$\max_{C_t, A_t} E_0 \sum_{t=0}^\infty \beta^t U(C_t)$$
$$\text{s.t. } C_t + A_t \leq Y_t + (1+r_t)A_{t-1} \quad \forall t$$

## Asset Demand Function
- Buying one more unit of $A_t$ requires one less unit of $C_t$
- $r_t$ more units of $A_t$ yield $1+r_t$ more units of $C_{t+1}$ in expected value
- $E_t[U'(C_{t+1})]$: expected marginal utility of $C_{t+1}$
- Discounted by $\beta$

## Combining the FOCs

$$\frac{U'(C_t)}{P_t} = \beta E_t \left[ \frac{U'(C_{t+1})}{P_{t+1}} (1+r_t) \right]$$

### Fisher Equation

$$1+i_t = (1+r_t)E_t \left[ \frac{P_{t+1}}{P_t} \right]$$


* Fisher Equation: Optimal choices of nominal and real assets 
		Result of the consumer's lagrangian 
	$1/(i+i_t) = E_t(i/(1+r_t) (P_t/P_{(t+1)} )$
	$i_t = r_t + E_t \pi_t$
		^ This makes sense. What is its implication though for the problem? 

Special Case:
- $\beta = \frac{1}{1+\rho}$
- $r_t = \rho$

$$U'(C_t) = \beta E_t[U'(C_{t+1})]$$

If $U(C_t) = \ln(C_t)$, then:

$$\frac{1}{C_t} = \beta E_t \left[ \frac{1}{C_{t+1}} \right]$$

## Solving the Difference Equation

$$C_{t+1} + A_{t+1} = Y_{t+1} + (1+r_t)A_t$$
$$C_{t+2} + A_{t+2} = Y_{t+2} + (1+r_t)A_{t+1}$$
$$\vdots$$
$$C_{t+s} + A_{t+s} = Y_{t+s} + (1+r_t)A_{t+s-1}$$

Solving for $A_t$:

$$A_t = \frac{1}{1+r_t} \left[ Y_{t+1} + A_{t+1} - C_{t+1} \right]$$

Iterating forward:

$$A_t = \sum_{s=1}^\infty \left( \frac{1}{1+r_t} \right)^s (Y_{t+s} - C_{t+s}) + \lim_{s \to \infty} \left( \frac{1}{1+r_t} \right)^s A_{t+s}$$

Dividing, we have connected $C_t$ and $Y_t$.

Because $Y_t$ is fluctuating, your decision of consumption would depend on $Y$ in the future, so we solve this difference equation.


# Information and Consumption

## Intertemporal Budget Constraint

$$\sum_{j=0}^\infty \beta^j E_t[C_{t+j}] = \frac{1}{P_t} \sum_{j=0}^\infty \beta^j E_t[Y_{t+j}] + (1+r_t)A_{t-1}$$

- All variables dated $t$, $t+1$, $t+2$, ... are stochastic processes
- Need to know the process of $Y_t$ here

### Assumptions on Income Process

$$Y_t = \bar{Y} + V_t$$
$$V_t \sim N(0, \sigma^2), \text{ i.i.d.}$$

$$E_t[Y_{t+j}] = \bar{Y}, \quad \forall j \geq 0$$

#### Implications
- $C_t = \bar{Y} + (1-\beta)V_t + (1+r_t)A_{t-1}$
  - Permanent Income: $\bar{Y}$
  - Transitory Income: $(1-\beta)V_t$
- Saving: $S_t \equiv Y_t - C_t = A_t - A_{t-1}$
  - MPC out of Permanent Income: 1
  - MPC out of Transitory Income: $1-\beta$