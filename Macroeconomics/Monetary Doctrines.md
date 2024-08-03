See [[Monetary Doctrines_ Summary]]
<span class="dark-mustard-text"> **</span>

Eric M. Leeper
University of Virginia 
Spring 2024
<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
## The Messages
1. ==A complete specification of macro policy is necessary for determination of equilibrium==
2. Complete specification includes enough information about policy behavior that agents can form expectations of the entire future paths of policy instruments
3. Monetary and fiscal policies must interact in certain ways in any equilibrium
4. ==Every statement about monetary policy effects is conditional on maintained assumptions about fiscal policy behavior==
5. And vice versa
<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
## <span class="dark-mustard-text"> The Model </span>

Prelims: 
* We are giving money more value here than what we did in the OLG. Rate or return on currency = Rate of return on loans. 
* Give money other role to play, total return: non pecuniary return + the original rate of return. This is monetary friction. 
* In infinite horizon models, we have to give money some other role, because the monetary rate of return is dominated by other assets because other assets are backed and money is not

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

- Draws on "Monetary Doctrines" in Ljungqvist-Sargent
- ==Shopping time monetary model==
	- constant endowment, $y > 0$ // helps us to get constant interest rates 
	- no uncertainty
	- steady-state analysis
	- lump-sum taxes/transfers
- ==How money gets valued unimportant to results==
- Aggregate resource constraint
$$c_t + g_t = y \quad (1)$$
- Preferences 
$$\sum_{t=0}^{\infty} \beta^t u(c_t, l_t), \quad 0 < \beta < 1 \quad (2)$$
$$u_c, u_l > 0; \quad u_{cc}, u_{ll} < 0, \quad u_{cl} \geq 0$$


<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
## Shopping Technology
- Households must ==spend time shopping==, $s_t$, to acquire consumption goods, $c_t$
- Endowed with unit of time 
- Shopping/transactions technology
$$s_t = H\left(c_t, \frac{m_t}{p_t}\right) \quad (3)$$
$m_t/p_t$ real money balances chosen at $t$
$H$ convex: $H, H_c, H_{cc}, H_{m/p m/p} \geq 0$, $H_{m/p}, H_{c,m/p} \leq 0$
- Example: Baumol-Tobin
$$H\left(c_t, \frac{m_t}{p_t}\right) = \frac{c_t}{(m_t/p_t)^\epsilon}, \quad \epsilon > 0$$
$\epsilon$: time cost per trip to the bank

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

## Other Constraints
- Time constraint
$$l_t + s_t = 1 \quad (4)$$
- Household budget constraint
$$c_t + \frac{b_t}{R_t} + \frac{m_t}{p_t} = y - \tau_t + b_{t-1} + \frac{m_{t-1}}{p_t} \quad (5)$$
$b$: 1-period indexed bonds; $p$: price level; $\tau$: lump-sum tax
- Maximize (2) s.t. (3), (4), (5)
- Note that
	- $m_t \geq 0$ (HH cannot issue currency)  // There will be a slackness condition 
	- $b_t \lessgtr 0$ (HH can borrow or lend)
- Multipliers: $\lambda_t$ for (5), $\mu_t$ for (4)
- write (4) as: $l_t + H(c_t, m_t/p_t) = 1$

## <span class="dark-mustard-text">Optimality Conditions</span> 

- FOC for $m_t/p_t$ is: $\lambda_t = \beta\lambda_{t+1} p_t/p_{t+1} - \mu_t H_{m/p}(t)$  
- Let $R_{mt} \equiv p_t/p_{t+1}$, the return on fiat currency // pecuniary return 
- Arbitrage between $m$ and $b$
#Ques: I have equal to sign not greater to sign in the following equation from my FOCs: 
$$1 - \frac{R_{mt}}{R_t} \geq -\frac{\mu_t}{\lambda_t} H_{m/p}(t) \geq 0$$
$$1 - \frac{R_{mt}}{R_t} = \frac{i_t}{1 + i_t} \geq 0 \quad (6)$$
- (6) leads to the key result that ==nominal interest rates are non-negative==:  
because $R_{mt} \leq R_t$ (currency is dominated in rate of return)
$i_t \geq 0$; $i_t$ is the nominal interest rate.  // It's always non-negative because storing currency is costless in this model. 

- Consumption-leisure tradeoff implies
$$\lambda_t = u_c(t) - u_l(t)H_c(t) \quad (7)$$
- From the FOC for $b_t$, return on bonds can be expressed as
$$R_t = \frac{1}{\beta}\left[\frac{u_c(t) - u_l(t)H_c(t)}{u_c(t+1) - u_l(t+1)H_c(t+1)}\right] \quad (8)$$
- (6) yields 
$$\left(\frac{R_t - R_{mt}}{R_t}\right) \lambda_t = -\mu_t H_{m/p}(t) \quad (9)$$

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
## <span class="dark-mustard-text">Money Demand</span>

- Combining FOCs [(7),(8),(9)] yields the ==implicit money demand==
$$\left(1 - \frac{R_{mt}}{R_t}\right) \left[\frac{u_c(t)}{u_l(t)} - H_c(t)\right] + H_{m/p}(t) = 0$$
- Evaluate $u_c(t), u_l(t)$ at $l_t = 1 - H(c_t, m_t/p_t)$ to get the implicitly defined money demand function
$$\frac{m_t}{p_t} = F\left(c_t, \frac{R_{mt}}{R_t}\right) = F(c_t, i_t) \quad (10)$$
- Straightforward to show in (10) that $F_c > 0$, $F_i < 0$; ==This is the general money demand relationship!== 

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

## <span class="dark-mustard-text">Government & Equilibrium </span> 

*(Capital letters when we are talking about the aggregates)*
- Government finances $\{g_t\}$ s.t.
$$g_t = \tau_t + \frac{B_t}{R_t} - B_{t-1} + \frac{M_t - M_{t-1}}{p_t} \quad (11)$$
- A price system is a pair of positive sequences $\{R_t, p_t\}_{t=0}^{\infty}$  
- Take as exogenous $\{g_t, \tau_t\}_{t=0}^{\infty}$ and $B_{-1} = b_{-1}$, $M_{-1} = m_{-1} > 0$.
#Ques: If Capital letters are aggregates, what are the small letters. What does B = b mean? 
An equilibrium is a price system, and sequences $\{c_t, B_t, M_t\}_{t=0}^{\infty}$ such that
	- the household's optimum problem is solved with $b_t = B_t$, $m_t = M_t$  
	- the government's budget constraint is satisfied
	- $c_t + g_t = y$

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

## <span class="dark-mustard-text">Policy Experiments </span> 
- Need a complete specification of policy
- Will give definite meaning to concepts of
	- "short run": initial date
	- "long run": stationary equilibrium
- Assume
	- $g_t = g \geq 0$  
	- $\tau_t = \tau \geq 1$
	- $B_t = B \geq 0$
- We permit $\tau_0 \neq \tau$, $B_{-1} \neq B$
- <span class="dark-mustard-text">Economy in stationary eqm for</span> $t \geq 1$ <span class="dark-mustard-text">but starts from a different position at </span> $t=0$
- Reduces dynamics to 2 periods: now ($t=0$) & future ($t \geq 1$)

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

## <span class="dark-mustard-text">Stationary Equilibrium </span>
- Seek an equilibrium with
	- $p_t/p_{t+1} = R_{m} \geq 0$
	- $R_t = R \geq 0$  
	- $c_t = c \geq 0$
which imply that
$$R = \beta^{-1}$$
$$\frac{m_t}{p_t} = F(c, R_m/R) = f(R_m), \quad f' > 0$$

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

## <span class="dark-mustard-text">Two Equilibrium Conditions</span>
1. Impose eqm on government budget constraint at $t \geq 1$
$$g - \tau + \frac{B(R-1)}{R} = f(R_m)(1 - R_m) \quad \text{(Future)}$$

(Total Seignorage Revenue)
2. Impose eqm on government budget constraint at $t=0$  
$$\frac{M_{-1}}{p_0} = f(R_m) - (g + B_{-1} - \tau_0) + \frac{B}{R} \quad \text{(Current)}$$
- Given $(g, \tau, B)$, (Future) $\Rightarrow R_m$—inflation rate
- Given $(g, \tau_0, B)$ & initial conditions $(M_{-1}, B_{-1})$, (Current) $\Rightarrow p_0$—initial price level
- Have completely determined eqm $\{p_t\}_{t=0}^{\infty}$
- Now consider alternative policies and how they affect price-level determination

Decisions today have to be consistent with future 
THE ABOVE TWO CONDITIONS COMPLETELY CHARACTERIZE THE EQUILIBRIUM. All other conditions are embedded here. 
<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

## Deriving Equilibria Graphically
![[monetary_doctrines_fig1.png]]
![[Pasted image 20240408141257.png]]
## 1. Sustained Deficits Cause Inflation
![[monetary_doctrines_fig2.png]]
Let $D = g - \tau + \frac{B(R-1)}{R}$ and consider $D' > D^*$

D is gross deficit. Added debt service. PV on the interest payment on the debt. 

// Two potential steady states: where inflation decreases and inflation increases. We rule that inflation decreases is an unstable equilibrium (we saw this in OLG). Learnability: People learn about what the equilibrium is, then you ll always converge to the other equilibrium. (??)

We get the classical doctrine under the condition that we have a stable equilibrium. 



## 1. Sustained Deficits Cause Inflation
![[monetary_doctrines_fig3.png]]
"normal" side: $D' > D^* \Rightarrow R'_m < R^*_m$ (classical doctrine)

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

* What are the fiscal requirements to target inflation? 

## 2. Zero Inflation Policy
- $\pi = 0 \Rightarrow R_m = 1 \Rightarrow \text{seigniorage} = 0$
- (Future) $\Rightarrow$
$$g - \tau + \frac{B(R-1)}{R} = 0$$
or
$$\frac{B}{R} = \frac{\tau - g}{R - 1} = \sum_{t=1}^{\infty} R^{-t}(\tau - g)$$
- Real value of interest bearing government debt = present value of net-of-interest primary surpluses
- Of course, this generalizes to any fixed inflation rate policy (e.g., inflation targeting)
- It is strange—and troubling—that no country that adopted inflation targeting simultaneously adopted fiscal policies that are consistent with it

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
(Leeper: The following is the most important paper in monetary and fiscal policy literature)
## 3. Unpleasant Monetarist Arithmetic  
- A little history—US FP in early 1980s
- Consider an open-market sale of bonds at $t=0$,
(M/P : Goods, Bonds are in real terms ) ; following is the definition of open market sale : CB sells bonds, people pay by currency
$$-d(M_0/p_0) = dB_0 > 0$$

!! CB removes from the public liabilities that earn $R_m$ and replaces those with liabilities that earn $R \geq R_m$. $\implies$ This generates fiscal consequences as it changes the asset set of the government, and what it owes to the people. !!

Fiscal Policy: 
- Hold fiscal policy—$(g, \tau_0, \tau)$—fixed $\implies$ Primary Deficit is constant 
- OM sale raises $B$ in eqm conditions (Current) & (Future)
- Higher debt service in the future, but FP fixed
- Future seigniorage must rise: $f(R_m)(1-R_m)$ rises by $\frac{R-1}{R}dB$
- Stationary $\pi$ rises ($R_m$ falls) unambiguously

$$\frac{M_{-1}}{p_0} = f(R_m) - (g + B_{-1} - \tau_0) + \frac{B}{R} \quad \text{(Current)}$$
- By (Current), effect on $p_0$ can be anything
	- What happens to $p_o$ depends on $f'(R_m)$ (interest elasticity of money demand)
	- if $f'(R_m)$ small, $p_0$ falls (usual result)
	- if $f'(R_m)$ large, $p_0$ rises (extreme unpleasantness)
	- Leeper: This result is not obvious in the IS-LM model 
- Tighter money via OMO—at best—temporarily lowers $p$ but at the cost of permanently raising $\pi$

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
## 4. Quantity Theory of Money
- Classic quantity theory of money experiment is a helicopter drop of money
- change $M_{-1}$ to $\lambda M_{-1}$, $\lambda > 0$
- holding fiscal policy—$(g, \tau_0, \tau, B)$—fixed
- By (Current), if $p_0 \to \lambda p_0$, then $M_{-1}/p_0$ unchanged
$$\frac{\lambda M_{-1}}{\lambda p_0} = f(R_m) - (g + B_{-1} - \tau_0) + \frac{B}{R} \quad \text{(Current)}$$
- Nothing happens to growth rate of money, $R_m$, or $\pi$
- Produces "neutrality of money" (not "superneutrality") #Ques: What is superneutrality of money? 
- Tobin's gremlins: required to leave portfolios unperturbed by $M$ drop
	- Tobin's critique was that money doesn't increase just by increasing money supply. Actual currency injection happens through instruments which changes stuff. 

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

## 5. A Neutral Open-Market Operation
- ==Redefine OMO from that used in unpleasant arithmetic to give MA fiscal powers so OMO have QT effects==
	// We are giving the Central Bank the fiscal power so as to not have the 'unpleasantness' of OMO. 
- Denote initial eqm by $\bar{x}$; new eqm by $\hat{x}$
- Consider OMO that decreases $M_0$ and increases $B$ and $\tau$ (with $\bar{\tau}_0 = \hat{\tau}_0$) such that
$$\left(1 - \frac{1}{R}\right)(\hat{B} - \bar{B}) = \hat{\tau} - \bar{\tau}$$
- If future taxes obey this for $t \geq 1$, then (Future) satisfied at initial $R_m$ (that is, $-d\tau + dB(1-1/R) = 0$)
- Highlights a key aspect of conventional MP analysis
	- lump-sum taxes in future adjust by just enough to service any additional interest payments arising from the OMO's effects on $B$
	- FP "held constant" via unchanged ==gross-of-interest deficit==
<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
## 6. The Optimum Quantity of Money
- Given stationary $(g, B)$, ==Friedman argued that agents are better off with higher stationary real money balances (ones associated with higher rates of return on money)==
// 
People are better off getting rid of this distortion: $R_m \geq R = \frac{1}{\beta}$ (See the last point for why)
If you increase $R_m$ $\implies$ decrease inflation. Printing money is cheap but there is cost to people if money is less. So print more money
//

Leeper: This will have fiscal consequences. Need to increase the taxes. 
- By running sufficiently large gross surpluses $(g - \tau + B(R - 1)/R < 0)$, government can attain any $R_m \in (1, 1/\beta)$
- #Ques: ^ Why is the range above limited? 
- So given $(g, B)$, choose $\tau$ to get required surplus to hit the target $R_m$
- ==Use proceeds of tax to retire currency (achieve negative growth of $M$)==
- Pursues Friedman's optimal policy of saturating economy with real balances
- ==Social value of real balances in model comes from reducing shopping time==
(Friedman: Have enough real balances that people don't waste time shopping)
- Optimum quantity of $M$ minimizes time spent shopping 
- Suppose there is a satiation point in real balances $\psi(c)$ for any $c$
$$H_{m/p}(c, m_t/p_t) = 0 \quad \text{for} \quad m_t/p_t \geq \psi(c)$$
- Can achieve this only by setting $R = R_m$ (since $\mu_t, \lambda_t > 0$)
- If $H(c, m/p) = \frac{c}{(m/p)}\epsilon$, can only approximate Friedman's rule since money demand insatiable

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
## 7. One Big Open-Market Operation
- Consider a large OM purchase of private indebtedness at $t=0$
	- gives government a portfolio of interest-earning claims on private sector
	- permits the government to run a gross-of-interest surplus (?)  
	- government uses surplus to reduce money supply and create deflation
	- this raises return on money $> 1$
	- idea underlies some optimal fiscal policy results
- Impose $g - \tau \geq 0$ so cannot achieve deflation through direct taxation
- Proposal: $M_0 \uparrow$, $B \downarrow$ with $B < 0$
- Given $(g, \tau)$, use (Future) to pick $B$ consistent with desired $R_m$ $(1 \leq R_m \leq 1/