<span class="dark-mustard-text">**</span>

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
## <span class="dark-mustard-text">Background</span>
- When taxes distort behavior, [[Ricardian equivalence]] breaks down
- <u>Distorting taxes</u> are proportional tax rates levied against labor earnings, saving, consumption, interest earnings, and so forth
- Taxes distort behavior whenever <u>tax rates directly affect the trade offs that agents face</u>
- ==How should the government optimally set tax rates that are distortionary?==
	- ==minimize distortions subject to given financing needs==
	- ==needs arise from spending & interest on debt==

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
## <span class="dark-mustard-text">Tax Distortions</span>
*This section shows why taxes are distortionary. They impact the choice between leisure and consumption.*
- Suppose consumers are choosing consumption, C, and leisure, l
- Taxes are levied against labor income and consumption at rates $\tau_L$ and $\tau_C$
- The consumer's budget constraint is: 
$$(1 + \tau_C)C = (1 - \tau_L)\frac{W}{P}(1 - l) + \Phi \tag{1}$$
- This implies the slope of the budget line in (C, l) space is:
$$\frac{dC}{dl} = -\frac{1 - \tau_L}{1 + \tau_C}\frac{W}{P}$$
	- higher $\tau_L$ reduces the opportunity cost of leisure
	- higher $\tau_C$ raises the cost of consumption

- Consumer maximizes $U(C, l) = \alpha \ln(C) + (1 - \alpha) \ln(l)$ subject to (1)
- First-order conditions imply: 
$$C = \frac{\alpha}{1 - \alpha}\frac{1 - \tau_L}{1 + \tau_C}\frac{W}{P}l$$
- ==This is the trade off consumers perceive between consumption & leisure==
	- both tax rates enter this trade off
	- when $\tau_L$ and $\tau_C$ are positive, the consumer's choices will be different than when the tax rates are zero
- This implies that taxes distort behavior
- ==In general, all taxes that governments can levy distort== (Eric mentioned how lump sum taxes are also distorting, I don't remember why though.)

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
## <span class="dark-mustard-text">A Model</span>
- We abstract from the specific taxes and their distortions
- We assume simply that collecting taxes is costly in the sense that it wastes resources
	- reflects the idea that higher tax rates create disincentives to work & invest  
- A representative consumer receives a constant endowment of Y goods each period
- Tax distortions serve to reduce the endowment according to the function $\psi(\tau_t)$
	- $\tau_t$ is tax revenue at t
	- $\psi(\cdot)$ is strictly increasing in $\tau_t$ at an increasing rate
	- $\psi(0) = 0$: no resources are wasted when revenue is zero
	- $\psi'(\tau_t) > 0$: as revenues rise, wasted resources rise  
	- $\psi''(\tau_t) > 0$: costs rise at an increasing rate

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
## <span class="dark-mustard-text">Consumer Behavior</span>
- The consumer real income is: 
$$y_t = Y - \psi(\tau_t)$$
- Their budget constraint is:
$$c_t + a_t = y_t + (1 + r_{t-1})a_{t-1}, \text{ given } a_{-1} > 0$$
- Consumer utility is:
$$U = E_0\sum_{t=0}^\infty \beta^t U(c_t) \quad 0 < \beta < 1$$
with $U(c_t) = c_t$, where $E_0$ is the mathematical expectation conditional on inflation at time 0
- Consumers choose $\{c_t, a_t\}$ to maximize utility subject to their budget constraint

- The Lagrangian is:
$$L = E_0\sum_{t=0}^\infty \beta^t\{c_t + \lambda_t[y_t + (1 + r_{t-1})a_{t-1} - c_t - a_t]\}$$
- Which yields the first-order conditions:
	- $1 = \lambda_t$  
	- $1 = \beta(1 + r_t)$
- Linear utility delivers constant marginal utility  
- We immediately get that the real interest rate is constant:
$$\frac{1}{1 + r_t} = \beta \quad \Rightarrow \quad r = \beta^{-1} - 1 = \rho \tag{2}$$
where $\rho$ is the rate of time preference
<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
## <span class="dark-mustard-text">Government Behavior</span>
- A benevolent government has a given sequence of purchases, $\{g_t\}$, that it seeks to finance using taxes and debt to maximize social welfare
- Social welfare is the lifetime utility, U of the representative consumer
- The goods market condition is that demand = supply:  
$$c_t + g_t = y_t = Y - \psi(\tau_t)$$
- Then the social welfare function comes from:
$$U(c_t) = c_t = y_t - g_t = Y - \psi(\tau_t) - g_t$$
$$U = E_0\sum_{t=0}^\infty \beta^t [Y - \psi(\tau_t) - g_t] \tag{3}$$
where government purchases, $g_t$, are given and not a choice for the government

- Government choices must be consistent with the budget identity:
$$\tau_t + b_t = g_t + (1 + r_{t-1})b_{t-1}, \quad b_{-1} = 0 \tag{4}$$
$b_t$: is one-period government debt that pays gross interest $(1 + r_t)$ at $t+1$
- The government chooses taxes and debt, $\{\tau_t, b_t\}$ to maximize social welfare, (3), subject to the budget identity, (4)
- The Lagrangian for the government is:
$$G = E_0\sum_{t=0}^\infty \beta^t \left[Y - \psi(\tau_t) - g_t  + \phi_t[g_t + \beta^{-1}b_{t-1} - b_t - \tau_t]\right]$$
where $\phi_t$ is the multiplier and $(1 + r_{t-1}) = \beta^{-1}$ (From the FOC's above)
- Equilibrium: consumer saving = government borrowing: $a_t = b_t$

- <span class="dark-mustard-text"> What does substituting </span>$1 + r_{t-1}$ with $\beta^{-1}$ mean?
	- the consumer's optimal choices imply the marginal rate of substitution is constant and equal to 1  
	- those choices require the real interest rate to be constant with 1 + r = \beta^{-1}  #Ques ❓
	- by making the substitution, we ensure that the government's choices are consistent with consumer optimizing behavior
	- It couldn't be otherwise
		- maximizing social welfare means maximizing the welfare of the representative consumer
		- if government made choices that required the interest rate to vary over time or to differ from \beta^{-1}, then the government couldn't be maximizing the consumer's welfare


- The government's first-order conditions with respect to $\tau_t$ and $b_t$ are: 
	- $-\psi'(\tau_t) - \phi_t = 0$
	- $-\phi_t + E_t\phi_{t+1} = 0$  
- What do these mean?
	- first: the benefit of relaxing the budget identity—for example, by raising revenues—equals the quantity of goods lost through tax distortions // <span class="dark-mustard-text">but what if they are raised by the debt? Why is it still equal? </span>: This is derivative wrt t so we are just looking at that. 	
	- second: the cost of relaxing the budget identity should be constant over time—that is, it should be smooth
- Taken together the first-order conditions imply the optimality condition:
$$\psi'(\tau_t) = E_t[\psi'(\tau_{t+1})] \tag{5}$$
- <span class="dark-mustard-text">marginal cost of taxes constant across time</span> $\implies$ This is the condition for the benevolent government trying to maximize the social welfare given having to raise $g_t$
<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
## <span class="teal-text">Optimal Policy </span> 
- When $\psi(\tau_t) = \phi\tau_t^2$, with $\phi > 0$, $\psi'(\tau_t) = 2\phi\tau_t$ and the optimality condition is:
$$\tau_t = E_t\tau_{t+1}$$
	- <span class="dark-mustard-text">tax smoothing implies no change in expected taxes</span>
	- akin to consumption smoothing, which gave $c_t = E_tc_{t+1}$

- $\psi(\tau_t) = \phi\tau_t^2$ implies setting taxes to satisfy $\tau_t = E_t\tau_{t+1}$
- By extension, $E_t\tau_{t+j} = \tau_t$  
- <span class="dark-mustard-text">Two questions remain:
	1. At what level should taxes be set?
	2. What role does government debt play in smoothing tax distortions?</span>
- Use the government budget identity:
$$\tau_t + b_t = g_t + (1 + r_{t-1})b_{t-1}, \quad b_{-1} = 0 \tag{4}$$
- Solve forward at time t, recognizing $r_t$ constant and future $g_{t+j}$ & $\tau_{t+j}$ unknown:
$$b_{t-1} = E_t\sum_{j=1}^\infty \frac{\tau_{t+j-1} - g_{t+j-1}}{(1+r)^j} = \frac{1}{1+r}E_t\sum_{j=0}^\infty \frac{\tau_{t+j} - g_{t+j}}{(1+r)^j} \tag{6}$$

(See [[Solving Difference Equations]])

- This says: ==value of bonds outstanding at beginning of t must be financed by future primary surpluses==
	- $\tau_{t+j} - g_{t+j}$: Primary Surplus: Income - Spending
*******
- Suppose government spending takes the simple form:
$$g_t = g + \varepsilon_t, \quad \varepsilon_t \sim \text{i.i.d.}, \quad E_t\varepsilon_{t+1} = 0$$
- $g$ is "permanent spending" & $\varepsilon_t$ is "temporary spending"
- We now can infer:
$$g_t = g + \varepsilon_t$$  
$$E_tg_{t+1} = g$$
$$\vdots$$  
$$E_tg_{t+j} = g$$

- We can now solve for the expected values of taxes and spending in (6)
- Breaking the right side into two bits:
$$\frac{1}{1+r}E_t\sum_{j=0}^\infty \frac{\tau_{t+j}}{(1+r)^j} = \frac{1}{1+r}\sum_{j=0}^\infty \frac{\tau_t}{(1+r)^j} = \tau_t\frac{1}{1+r}\sum_{j=0}^\infty \left(\frac{1}{1+r}\right)^j = \tau_t\frac{1}{1+r}\frac{1}{1-\frac{1}{1+r}} = \frac{1}{r}\tau_t$$
$$\frac{1}{1+r}E_t\sum_{j=0}^\infty \frac{g_{t+j}}{(1+r)^j} = \frac{1}{1+r}\left[(g + \varepsilon_t) + \sum_{j=1}^\infty \left(\frac{1}{1+r}\right)^j g\right] = \frac{1}{1+r}\left[(g + \varepsilon_t) + \frac{1}{1+r}\sum_{j=0}^\infty \left(\frac{1}{1+r}\right)^j g\right] = \frac{1}{r}g + \frac{1}{1+r}\varepsilon_t$$

- Substitute these results into (6) and solve for the optimal tax rule:
$$\tau_t = g + \frac{r}{1+r}\varepsilon_t + rb_{t-1} \tag{7}$$
- Can infer marginal propensity to tax (MPT):
	1. MPT for permanent spending = 1
	2. MPT for temporary spending $\frac{r}{1+r} \ll 1$  
	3. MPT for debt service r, just cover interest payments
- (7) is the rule for setting taxes optimally when government spending is a constant plus a mean zero random variable

- To derive the implications of the optimal tax rule for government debt, use the rule, (7) in the budget identity, (4):
$$b_t + \tau_t = g_t + (1+r)b_{t-1} \tag{4}$$
$$b_t + g + \frac{r}{1+r}\varepsilon_t + rb_{t-1} = g_t + rb_{t-1}$$
$$b_t = \frac{1}{1+r}\varepsilon_t + b_{t-1} \tag{8}$$
- Last expression—the debt rule, (8)—says:
	1. Do not issue debt to finance permanent spending, g
	2. Issue enough debt to finance a large fraction of the change in transitory spending, $\frac{1}{1+r}\varepsilon_t$ (because r small)  
	3. In the absence of changes in transitory spending, $\varepsilon_t = 0$, keep debt constant, $b_t = b_{t-1}$


<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
Key Takeaways
<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>


![[Econ7040S24TaxandInflationSmoothing.pdf]]

Other: [[Tax Smoothening]]
