

## <span class="dark-mustard-text">Overview</span>

- These notes extend OLG models in two ways
    1. ==Permit heterogeneity within a generation
        - tractable way to get trade
        - permits study of "inside money"
    2. Introduce fiat currency
        - unbacked currency as "social contrivance"
        - conditions for existence of monetary equilibrium
        - ==fiat currency may improve efficiency==

when currency is valued it is a bubble  
==Its value exceeds the value of its dividend stream which is 0==

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

## <span class="dark-mustard-text">Setup</span>

- time discrete, $t = 1, 2, \ldots$
- at $t$, $N_t$ two-period-lived agents born
- endowed with consumption goods, $(w_t^{y(h)}, w_{t+1}^{o(h)})$
- preferences of generation $t$ are $u^h(c_t^{y(h)}, c_{t+1}^{o(h)})$
	$h$ is the cohort
- $u(\cdot, \cdot)$ has usual properties plus $$v(c^y, c^o) \equiv \frac{\partial u/\partial c^y}{\partial u/\partial c^o}$$ $$\lim_{c^y \to 0} v(\cdot) = \infty \text{ for } c^o > 0$$  
    $$\lim_{c^o \to 0} v(\cdot) = 0 \text{ for } c^y > 0$$
- $(h)$ distinguishes among agents within a generation to allow for differences across agents
- ==differences will be primarily in endowments==


<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

## <span class="dark-mustard-text">Agents' Problem</span>

- Agents may trade consumption loans, $l_t^{y(h)}$, which yield gross real interest of $(1 + r_t)$
    - $l_t^{y(h)} > 0$: young agents at $t$ from cohort $h$ lend goods
- Members of generation $t$ maximize $u^h(c_t^{y(h)}, c_{t+1}^{o(h)})$ subject to $$c_t^{y(h)} + l_t^{y(h)} = w_t^{y(h)} - \tau_t^{y(h)}$$ $$c_{t+1}^{o(h)} = w_{t+1}^{o(h)} - \tau_{t+1}^{o(h)} + (1 + r_t)l_t^{y(h)}$$ $\tau$'s are lump-sum taxes net of transfers;  
    $c_t^{y(h)} \geq 0$, $c_{t+1}^{o(h)} \geq 0$ and $l_t^{y(h)}$ unconstrained
- Old at $t = 1$ endowed $w_1^{o(h)}$ and maximize $c_1^{o(h)}$
- Combine (1) and (2) to get agents' intertemporal budget $$c_t^{y(h)} + \frac{c_{t+1}^{o(h)}}{1 + r_t} = w_t^{y(h)} - \tau_t^{y(h)} + \frac{w_{t+1}^{o(h)} - \tau_{t+1}^{o(h)}}{1 + r_t}$$
- Aggregate resource constraint $$G_t + \sum_h c_t^{y(h)} + \sum_h c_t^{o(h)} = \sum_h w_t^{y(h)} + \sum_h w_t^{o(h)}$$ $G_t$ is government purchases, thrown in ocean
- Government budget identity $$G_t + L_t^g = \sum_h \tau_t^{y(h)} + \sum_h \tau_t^{o(h)} + (1 + r_{t-1})L_{t-1}^g, \quad t \geq 1$$ $L_t^g > 0$: government lending to agents; $L_0^g = 0$

- Agent $h$'s Lagrangian with multipliers $\lambda_t^{y(h)}$ (on (1)) and $\lambda_{t+1}^{o(h)}$ (on (2)); FOC's $$c_t^{y(h)}: u_1^h(c_t^{y(h)}, c_{t+1}^{o(h)}) = \lambda_t^{y(h)}$$  
    $$c_{t+1}^{o(h)}: u_2^h(c_t^{y(h)}, c_{t+1}^{o(h)}) = \lambda_{t+1}^{o(h)}$$  
    $$l_t^{y(h)}: \lambda_t^{y(h)} = (1 + r_t)\lambda_{t+1}^{o(h)}$$
- Combine these to yield $$\frac{1}{1 + r_t} = \frac{u_2^h(c_t^{y(h)}, c_{t+1}^{o(h)})}{u_1^h(c_t^{y(h)}, c_{t+1}^{o(h)})}$$

- Assume
    1. consumption goods are normal goods
    2. $(c_t^{y(h)}, c_{t+1}^{o(h)})$ gross substitutes: income effect does not dominate substitution effect from change in $r_t$
- FOCs and (1) imply saving function, $l_t^{y(h)}$ $$l_t^{y(h)} = f_t^h \left[ \stackrel{(+)}{r_t}, \stackrel{(+)}{w_t^{y(h)} - \tau_t^{y(h)}}, \stackrel{(-)}{w_{t+1}^{o(h)} - \tau_{t+1}^{o(h)}} \right]$$
- Aggregate agents' budget constraints, (1) and (2)  
    young at $t$: $\sum_h c_t^{y(h)} + \sum_h l_t^{y(h)} = \sum_h w_t^{y(h)} - \sum_h \tau_t^{y(h)}$  
    old at $t$: $\sum_h c_t^{o(h)} = \sum_h w_t^{o(h)} - \sum_h \tau_t^{o(h)} + (1 + r_{t-1}) \sum_h l_{t-1}^{y(h)}$


- Combine ARC (4) and GBI (5) and employ the aggregated budget constraints to yield $$L_t^g + \sum_h l_t^{y(h)} = (1 + r_{t-1}) \left[ L_{t-1}^g + \sum_h l_{t-1}^{y(h)} \right], \quad t \geq 1$$ with the initial condition $L_0^g = \sum_h l_0^{y(h)} = 0$
- The unique solution is $$L_t^g + \sum_h l_t^{y(h)} = 0, \quad t = 0, 1, 2, \ldots$$

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

## <span class="dark-mustard-text">Equilibrium</span>

An equilibrium is a collection of sequences ${N_t, w_1^{o(h)}, w_t^{y(h)}, w_{t+1}^{o(h)}, \tau_1^{o(h)}, \tau_t^{y(h)}, \tau_{t+1}^{o(h)}, c_1^{o(h)}, c_t^{y(h)}, c_{t+1}^{o(h)}, l_t^{y(h)}, r_t, G_t, L_t^g}$ such that

1. Given ${r_t}_{t=1}^\infty$, consumption allocations, ${c_t^{y(h)}, c_{t+1}^{o(h)}}_{t=1}^\infty$, and lending, ${l_t^{y(h)}}_{t=1}^\infty$, solve agent $h$'s problem to maximize $u^h(c_t^{y(h)}, c_{t+1}^{o(h)})$ subject to (1) and (2).
2. The government budget identity, (5), is satisfied for $t \geq 1$, with $L_0^g = 0$.
3. The loan market clears to satisfy (9) for $t \geq 1$.

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

## <span class="dark-mustard-text">Example</span>

- Assume
    1. $u^h(c_t^{y(h)}, c_{t+1}^{o(h)}) = \ln c_t^{y(h)} + \ln c_{t+1}^{o(h)}$
    2. $N_t = N_1 + N_2$ for $t \geq 1$
    3. $N_1$ lenders endowed $(w_t^{y(h)}, w_{t+1}^{o(h)}) = (\alpha, 0)$, $\alpha > 0$
    4. $N_2$ borrowers endowed $(w_t^{y(h)}, w_{t+1}^{o(h)}) = (0, \beta)$, $\beta > 0$
    5. $G_t = 0$ for $t \geq 1$ and guess one solution for taxes is $(\tau_t^{y(h)}, \tau_{t+1}^{o(h)}) = (0, 0)$ for all $h$ and $t \geq 1$
    6. Restrict $\tau_1^{o(h)} \leq 0$ (initial old receive transfers)
- Government budget identity is  
    $$L_1^g = \sum_h \tau_1^{o(h)} \leq 0$$ $$L_t^g = (1 + r_{t-1})L_{t-1}^g, \quad t \geq 2$$

- Loan supply & consumption of young are | Lenders | Borrowers | |:-------:|:---------:| | $l_t^{y(h)} = \frac{\alpha}{2}$ | $l_t^{y(h)} = -\frac{\beta}{2(1 + r_t)}$ | | $c_t^{y(h)} = \frac{\alpha}{2}$ | $c_t^{y(h)} = \frac{\beta}{2(1 + r_t)}$ |
- Loan market equilibrium $$N_1 \frac{\alpha}{2} - N_2 \frac{\beta}{2(1 + r_t)} + L_t^g = 0$$
- This yields the equilibrium interest rate $$1 + r_t = \frac{N_2 \beta}{N_1 \alpha + 2L_t^g} \equiv \left( \frac{\text{borrowing}}{\text{lending}} \right)$$
- An equilibrium is $\tau_1^{o(h)} \leq 0$ and ${L_t^g, 1 + r_t}$ satisfying (10)-(12)
- One solution is $\tau_1^{o(h)} = 0$ for all $h$, $L_t^g = 0$ for all $t$, and  
    $$1 + r_t = \frac{N_2 \beta}{N_1 \alpha}$$
- If $N_2 \beta / N_1 \alpha \geq 1$, this is the unique equilibrium: reasoning
    1. when $N_2 \beta / N_1 \alpha \geq 1$, $L_1^g = \sum_h \tau_1^{o(h)} < 0$ implies  
        $$1 + r_t > 1 + r_{t-1} > \ldots > 1 + r_1 > 1$$  
        and  
        $$L_t^g < L_{t-1}^g < \ldots < L_1^g < 0$$ $\implies$ government borrows without bound
    2. eventually, $L_t^g$ will exceed $N_1 \alpha$ in absolute value
    3. government is borrowing with no tax backing
    4. then (12) cannot be satisfied by any positive $1 + r_t$
    5. $\therefore N_2 \beta / N_1 \alpha \geq 1 \implies$ no equilibrium exists with $L_1^g < 0$
- When $N_2 \beta / N_1 \alpha < 1$, there can be many equilibria

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

## <span class="dark-mustard-text">Adding Currency</span>

- We extend the model to include both unbacked currency and government bonds, to permit analysis of open-market operations
- At beginning of time 1, government has $H_1 > 0$ units of "dollars"
- Let $p_t$ be the price level at $t$, in dollars per time-$t$ good
- Government budget identity is $$G_t = \sum_h \tau_t^{y(h)} + \sum_h \tau_t^{o(h)} + (1 + r_{t-1})L_{t-1}^g - L_t^g + \frac{H_t - H_{t-1}}{p_t}$$ where $H_0 = 0$ and $H_t \geq 0$. $p_t = +\infty$ for all $t \geq 1$ means currency not valued and (13) collapses to (5)
- Three potential stores of value: private loans, government loans, currency (if $p_t < +\infty$)

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

fhgjryh

## <span class="dark-mustard-text">Open-Market Operations in Government Bonds</span> 

- We can now state a proposition due to Neil Wallace ==that government open-market operations in currency and government bonds *may be* irrelevant for determining prices and allocations.==

- **Proposition 2.** Under the assumptions of Proposition 1, there exist many currency equilibria. Let $\bar{p}_t$ be the equilibrium price level for Proposition 1. 
- For a fixed value of $H_1 > 0$ and fixed settings of the fiscal variables $\{G_t, \tau_t^{o(h)}, \tau_t^{y(h)}, t \geq 1\}$, there exist a continuum of equilibria, all with a price-level sequence $\bar{p}_t$ of the Proposition 1 equilibrium, but with different values for $H_t$, $t \geq 2$, and $L_t^g$, $t \geq 2$. For $t \geq 2$, the values of $L_t^g$ and $H_t$ can be arbitrary, so long as they obey $H_t > 0$ and the constraint on open-market operations that
    $$-L_t^g + \frac{H_t}{p_t} = -\bar{L}_t^g \tag{17}$$
    or, equivalently, $-dL_t^g + d(H_t/p_t) = 0$.

- The proof of this is straightforward and left to you
- ==Central to this proposition is that bonds and currency pay the same rate of return, so currency is *not* dominated in rate of return==

- Let total tax revenue be $T_t = \sum_h \tau_t^{o(h)} + \sum_h \tau_t^{y(h)}$
- ==Fixed fiscal policy means the primary deficit, $D_t = G_t - T_t$, is unchanged by open-market operations==, with implications for equilibrium conditions
    1. government budget identity, (15), becomes
        $$D_t = (1 + r_{t-1})\left(L_{t-1}^g - \frac{H_{t-1}}{p_{t-1}}\right) - \left(L_t^g - \frac{H_t}{p_t}\right)$$
        with $D_t$ fixed (because fiscal variables unchanged)
    2. loan market equilibrium, (16), becomes
        $$\sum_h l_t^{y(h)} = -L_t^g + \frac{H_t}{p_t}$$
        with $\sum_h l_t^{y(h)}$ fixed (because $r_t$, $\tau_t^{y(h)}$, $\tau_t^{o(h)}$ unchanged)

- Any policy that satisfies $-dL_t^g + d(H_t/p_t) = 0$ continues to satisfy these conditions

<span class="dark-mustard-text">This is happening because the two assets are perfect substitutes. </span> This is not how the world works but starting point and then find how it works. 

- Wallace's paper was entitled "A Modigliani-Miller Theorem for Open-Market Operations"
	- Modigliani-Miller Theorem: It doesnt matter if a firm uses equity or debt to finance its costs. 
- Title stems from the fact that in this model agents are indifferent between holding their saving in government bonds or currency
- This is a form of the Modigliani-Miller theorem that a firm's value does not depend on the firm's financing (under certain conditions)
- Here that logic is applied to the composition of agents' saving portfolios
- We will see that the assumption about fiscal behavior is critical to the outcome
- This theme—that monetary policy impacts depend on assumptions about fiscal behavior (and vice versa)—runs through the macro policy literature
- <span class="dark-mustard-text">Money here is being injected through asset purchase and sell. It matters how the money is injected. </span>
<span class="dark-mustard-text">**</span>

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

##  <span class="dark-mustard-text">Open-Market Operations in Private Claims</span>

 * <span class="dark-mustard-text"> Should not matter if you keep the backing fixed. </span>

- Consider an equilibrium in Proposition 2 in which $L_t^g = 0$ (government is not doing any borrowing or lending)so real balances are
    
    $\sum_h l_t^{y(h)} = \bar{L}^g_t$
    
    $$\frac{\bar{H}_t}{\bar{p}_t} = -\bar{L}_t^g > 0$$
    where $\bar{L}_t^g$ is net government borrowing described in Proposition 1

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

- Let $\hat{H}_t$, $\hat{L}_t^g$ be currency & government loans in another Proposition 2 equilibrium with $\hat{L}_t^g > 0$
- Proposition 2 implies
    $$\frac{\hat{H}_t}{\bar{p}_t} = \frac{\bar{H}_t}{\bar{p}_t} + \hat{L}_t^g , \ t \geq 1 \tag{18}$$
    because $\hat{L}_t^g > 0$, $\hat{H}_t > \bar{H}_t$
- ==Government issues currency to purchase private loans: part of the currency is backed by private loans (endowments)==
- We show that $\bar{P}_t$ stays constant from the Prop 2. 


- Higher $H_t$ used to <u>buy private debt instruments have no effect on equilibrium </u>  $p_t$

- This illustrates the *real bills doctrine* that central bank purchases of private loans leave equilibrium allocations and prices unchanged

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

Real Bills Doctrine: 

Total liabilities of the Central Bank 
$\frac{\hat{H}}{\bar{P}_t} > \hat{L}^g_t$ by the amount $\frac{\bar{H}}{\bar{P}_t}$
* CB's net worth is -$\frac{\bar{H}}{\bar{P}_t}$
* What does it mean by a negative net worth of CB? It means that the CB cannot give remittances to the treasury until this is sorted. !Understand this more!!! 

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

- Variations in stock of currency backed by privately issued claims have no price-level effects
- Variations in stock of currency not fully backed affect price level
    - in the proof to Proposition 1: have a distinct $p_1$ and $p_t$ path for every $H_1 > 0$
    - initial price level comes from
        $$p_1 = \frac{H_1}{\sum_h l_1^{y(h)}}$$  
    - subsequent $p_t$'s come from
        $$\frac{p_t}{p_{t+1}} = 1 + \bar{r}_t$$

- Message: effects of currency stock on $p_t$ depend on what happens to government-held assets
    - including prospective tax receipts


MAJOR TAKEAWAY: Currency always matter on the backing 

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
## <span class="dark-mustard-text">Computing Equilibria</span>

- To compute solutions & examine optimality, it's helpful to establish some notation
- Population evolves as
    $$N_t = (1 + n)N_{t-1}, \ t \geq 1, \ n > -1 \tag{19}$$
    with $N_0 > 0$ given

- Assume endowments & taxes imply that per capita saving is a <u>time-invariant function</u> of $1 + r_t$; denote per capita aggregate private saving
    $$f(1 + r_t) \equiv \frac{\sum_h f_t^{(h)}[1 + r_t, w_t^{y(h)} - \tau_t^{y(h)}, w_{t+1}^{o(h)} - \tau_{t+1}^{o(h)}]}{N_t}$$
    Assume $f' > 0$ (saving monotonically increasing in interest rate)

- Let $h_t$ be per capita real government indebtedness (combining two kinds of government indebtedness): 
    $$h_t \equiv \frac{-L_t^g + \frac{H_t}{p_t}}{N_t} \tag{20}$$

- Let $d_t$ be per capita real primary government budget deficit
    $$d_t \equiv \frac{G_t - T_t}{N_t} \tag{21}$$

- (20) and (21) imply the government budget identity
(This is an accounting equation) 
    $$h_t = \left(\frac{1 + r_{t-1}}{1 + n}\right)h_{t-1} + d_t, \ t \geq 1 \tag{22}$$
    with $h_0 = 0$

- The loan market clearing condition is
    $$h_t = f(1 + r_t), \ t \geq 1 \tag{23}$$

- (22) and (23) determine $\{h_t, 1 + r_t; t \geq 1\}$ given exogenous $\{d_t; t \geq 1\}$ (exogenous deficits)

- Sargent (1987, chapter 7), *Dynamic Macroeconomic Theory*, offers general analyses of the system in (22) and (23)
- Note that loan market clearing implies
    $$1 + r_{t-1} = f^{-1}(h_{t-1})$$

- Dynamics then reduce to a single equation
    $$h_t = \left(\frac{f^{-1}(h_{t-1})}{1 + n}\right)h_{t-1} + d_t, \ t \geq 2, \ h_1 = d_1$$

- We now turn to interpreting currency equilibria

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
## <span class="dark-mustard-text">Currency Equilibria</span>

- Set $L_t^g = 0$, all $t \geq 0$ so that $h_t \geq 0$, all $t$, and all government debt is in currency
- Now, $h_t = H_t/p_t N_t$, $t \geq 1$ and no-arbitrage implies
    $$1 + r_t = \frac{p_t}{p_{t+1}}, \ t \geq 1, \text{ when } 0 < p_t < +\infty$$
- $1 + n$ is the Wicksellian =="natural rate of interest"==

## Aggregate Saving

- $f(1 + r_t)$ denotes aggregate per capita saving correspondence; $f' > 0$

![[Pasted image 20240327151522.png]]

<div style="border-bottom: 5px solid #00FFFF; margin: 10px 0;"></div>
## Case 1: Temporary Deficit

$d_t = \frac{G_t - T_t}{N_t}$


- Assume $f(1 + n) > 0$ (private sector saves) and $d_1 \geq 0$ and $d_t = 0$ for $t \geq 2$
- At $t = 1$, government offers to exchange $H_1$ units of currency for goods at price $p_1$
- After $t = 1$, government abstains from creating currency, so $H_t = H_1$, $t \geq 2$ & $d_t = 0$, $t \geq 2$
- Value of $d_1$ determined by $p_1$; $p_1$ *is determined by household behavior* . 
	- If the private sector does not want to lend, $d_t = 0$
- ==One stationary equilibrium (point B on figure)==: $p_t = +\infty$ (because H>0) and $h_t = h_{t-1} = 0$, $t \geq 1$
- ==Another stationary equilibrium (point A on figure)== comes from the solution to $h_1 = H_1/p_1 N_1 = f(1 + n)$ or
    $$p_1 = \frac{H_1}{N_1 f(1 + n)} \equiv p_1^* \tag{24}$$
    $$1 + n = \frac{p_t}{p_{t+1}}, \ t \geq 1 \tag{25}$$
- Any $p_1 > p_1^*$ in (24) is also an equilibrium price level, which results in $h_t < f(1 + n)$ and $\lim_{t \rightarrow \infty} h_t = 0$
![[Pasted image 20240401141149.png]]
- At $h_1$ (point A): $p_1 = p_1^*$, $1 + r_{t-1} = 1 + n$, to yield stationary equilibrium (24) & (25)
- At $h_1''$ (point B): $p_1 > p_1^*$, $1 + r_{t-1} < 1 + n$, so $\lim_{t \rightarrow \infty} h_t = 0$ and converge to non-currency equilibrium (non-monetary equilibrium \implies currency has no equilibria)
- At $h_1'$: $p_1 < p_1^*$, $1 + r_{t-1} > 1 + n$, so $\lim_{t \rightarrow \infty} h_t = +\infty$ and no stationary equilibrium exists

#Ques: $p_1 < p_1^*$, $1 + r_{t-1} > 1 + n$, How do we know this?  ; h = H/P_t. H constant. So if P-t goes up, h goes down and then look at the graph pls! 
#Quest Why is point A a stationary equilibrium? Is it because d_t = 0? 
<span class="dark-mustard-text">*We are looking at equation 22 for these limits* 
*Once you have the price level, everything follows from that.* </span>
## <span class="dark-mustard-text">Case 1: Temporary Deficit Example</span>

- Preferences: $u^h(c_t^{y(h)}, c_{t+1}^{o(h)}) = \ln c_t^{y(h)} + \ln c_{t+1}^{o(h)}$
- Endowments: $w^y = \sum_h w_t^{y(h)}/N_t$, $w^o = \sum_h w_{t+1}^{o(h)}/N_t$, $w^y > w^o$
- Yields per capita aggregate saving function
    $$f(1 + r_t) = \frac{w^y}{2} - \frac{w^o}{2(1 + r_t)}$$

- Equilibrium condition for loans $f(1 + r_t) = H_t/p_t N_t$
    $$\frac{H_1}{p_t N_t} = \frac{w^y}{2} - \frac{w^o}{2}\frac{p_{t+1}}{p_t}$$

- Write as difference equation in $p_t$  
    $$p_t = \frac{2}{w^y}\frac{H_1}{N_t} + \frac{w^o}{w^y} p_{t+1}$$

We iterate forward here. Economically, we do so because agents are forward looking, they save in currency while young and they are concerned about their return in old age depend on $P_{t+1}$

#Ques How does higher H1 lead to higher Pt but lower value of the asset? H is constant, so H has lower purchase value. 


- General solution is
    #Ques Learn how to do this? 
    $$p_t = \frac{2}{w^y} \sum_{s=0}^\infty \left(\frac{w^o}{w^y}\right)^s \frac{H_1}{N_{t+s}} + c \left(\frac{w^y}{w^o}\right)^t \ t \geq 1$$
    for any constant $c$ of integration
When you put c=0, you are putting this on stable manifold. #Ques What does it mean? 



- Let $N_t = (1 + n)N_{t-1} = \theta N_{t-1}$ to get
    $$p_t = \frac{2}{w^y} \sum_{s=0}^\infty \left(\frac{w^o}{w^y \theta}\right)^s \frac{H_1}{N_t} + c \left(\frac{w^y}{w^o}\right)^t \ t \geq 1$$

- Infinite sum converges when $w^o/w^y \theta < 1$ to. #Ques What is it greater than 1? Can it not converge to a negative number?  Infinite sum formula
    $$p_t = \frac{2}{w^y} \left(\frac{1}{1 - \frac{w^o}{w^y \theta}}\right) \frac{H_1}{N_t} + c \left(\frac{w^y}{w^o}\right)^t$$

- Solutions for $p_t$ satisfy $0 < p_t < +\infty$ for $1 \leq t \leq \infty$ for any $c \geq 0$
    - $c$ is arbitrary and indexes the continuum of equilibria
    - $c = 0$ delivers the stationary equilibrium
    - when $c > 0$, $\lim_{t \rightarrow \infty}(p_t/p_{t+1}) = w^o/w^y$ the equilibrium gross interest rate for the economy without valued currency
#Ques <span class="dark-mustard-text">What part of the model assumptions make people more uncertain about price's value over time? In reference to the coefficient for $c$? </span> 


- Can you ascribe economic intuition to the constant $c$?
    - how does $c$ arise mathematically?
    - how does the math relate to the agents' saving behavior or expectations formation?
    - (don't forget that this is a perfect foresight equilibrium, so expectations still play a central role)

<span class="dark-mustard-text"> * </span> 

<div style="border-bottom: 5px solid #00FFFF; margin: 10px 0;"></div>
## <span class="dark-mustard-text">Case 2: Permanent Deficit </span> 

- Assume $d_t = d > 0$ for $t \geq 2$ // Constant deficit! 
- Treat $t = 1$ deficit as endogenous, determined by
    $$d_1 = h_1 = \frac{H_1}{p_1 N_1}$$
    - if $p_1 = +\infty$, deficit cannot be financed because currency has no value
    - for any $p_1 < +\infty$, deficit can be financed by new currency creation, according to (22)

- Combine the loan market equilibrium condition, $f(1 + r_t) = h_t$, and the dynamics of $h_t$ from the government's budget identity $h_t = \left(\frac{f^{-1}(h_{t-1})}{1 + n}\right)h_{t-1} + d$

- Write real balance dynamics as $h_t = \left(\frac{f^{-1}(h_{t-1})}{1 + n}\right)h_{t-1} + d = \phi(h_{t-1}) + d$, where $\phi(h_{t-1}) \equiv \left(\frac{f^{-1}(h_{t-1})}{1 + n}\right)h_{t-1}$

<div style="border-bottom: 1px solid #00FFFF; margin: 10px 0;"></div>

- Note that:
	- $\phi'(h_{t-1}) > 0$ (show it)
	- $\phi'(0) = \frac{f^{-1}(0)}{1+n}$
	- $\phi(h_{t-1})$ ==has an asymptote at the upper bound on per capita saving== #Ques What does it mean? Why does it matter? 

### The next figure shows the case if $\frac{f^{-1}(0)}{1+n} < 1$ and $d$ sufficiently small
- Two stationary points satisfy (22) and (23) with $h_{\infty} = h_t$ and $r_{\infty} = r_t$ for all $t$:
	- $d = h_{\infty}\left(\frac{n - r_{\infty}}{1 + n}\right)$
	- $h = f(1 + r_{\infty})$
- One stationary point is stable; the other is unstable

![[Pasted image 20240401150141.png]]

* Stationary points lie at the 45 degree line as h_t = h_{t-1}
* If d is too big, it would never intersect with the 45 degree line so no stationary equilibria #Ques : But it could still have an equilibrium right? 

- $\phi(h_1^{\infty})$ stable
- $\phi(h_2^{\infty})$ unstable
Why? 
<span class="dark-mustard-text">the slope at h1 is less than 1</span> $\implies$ eq 22 difference equation is stable and vice verse 


Laffer curve: depicts the relationship between tax rates and the revenue the government receives


![[Pasted image 20240401151110.png]]

Tax is inflation 
Revenue is money balances 
// Understand this last step more
tax base (labor income// h)* tax rate 

#Ques Is there stable/unstable in laffer curve? 




## Optimality

- Close connection between the conditions under which there fails to exist an optimal equilibrium without currency and under which there exists an equilibrium with valued currency
- Suppose young agents have identical preferences & endowments and $N_t = (1 + n)N_{t-1}$, $t \geq 1$
- Aggregate saving, $f(1 + r_t)$, is also the representative agent's saving
- Assume $G_t = 0$, $t \geq 1$
- The equilibrium interest rate for economy without valued currency is determined by $f(1 + r_t) = 0$
	- because $f$ is time invariant, $1 + r_t = 1 + r$, $t \geq 1$

- Proposition. If $1 + r < 1 + n$, the equilibrium is not Pareto optimal.
- Proof: We assume that $1 + r < 1 + n \equiv \theta$ and construct a feasible consumption allocation that Pareto dominates the equilibrium allocation. A superior allocation comes from redistributing at least some goods from young to old for each generation. We will make use of the figure that follows.

- In the figure, let the equilibrium consumption allocation be $(c_t^{y(h)}, c_{t+1}^{o(h)}) = (\bar{c}^y, \bar{c}^o)$ for all $h$ and all $t \geq 1$ and $c_1^{o(h)} = \bar{c}_1^o$ for all $h$
- Because this allocation is feasible, it satisfies $N_t \bar{c}^y + N_{t-1} \bar{c}^o = Y_t$, where $Y_t = \sum_h w_t^{y(h)} + \sum_h w_{t+1}^{o(h)} = N_t w^y + N_{t-1} w^o$
- Consider the alternative allocation $c_1^{o(h)} = \bar{c}_1^o + \theta\varepsilon$, $(c_t^{y(h)}, c_{t+1}^{o(h)}) = (\bar{c}^y - \varepsilon, \bar{c}^o + \theta\varepsilon)$
	- for any $\varepsilon > 0$, this is preferred by the old of generation 0
	- can choose an $\varepsilon > 0$ so the allocation is preferred by all generations born in $t \geq 1$
	- this moves southeasterly along line with slope $-1/(1 + n) = -\theta^{-1}$ through $(\bar{c}^o, \bar{c}^y)$
	- confirm candidate allocation is feasible

- Individual $h$'s consumption allocations [image omitted]

- We showed that when $1 + r < 1 + n$, can find Pareto improvement
- When $f' > 0$ everywhere, the condition that the solution for $r$ to $f(1 + r) = 0$ satisfies $1 + r < 1 + n$ is equivalent to $f(1 + n) > 0$
- These results generalize, as Balasko-Shell have shown

## Suggestions For Studying

1. Derive every expression on your own
2. Write—in words—your interpretation of the economics contained in the math
3. When possible, show the analysis graphically
4. In your interpretations be sure to differentiate between individual behavior and equilibrium outcomes
5. Create your own examples by assuming particular utility functions and endowment/taxation patterns.
6. Experiment with policies not examined in these slides, e.g., changes in $G_t$
7. Using an example economy, explicitly illustrate Propositions 1 and 2
8. Can you think of alternative ways to specify open-market operations in government bonds and currency such that those operations affect equilibrium allocations and/or prices?