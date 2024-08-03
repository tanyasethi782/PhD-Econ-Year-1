<span class="dark-mustard-text">**</span>
## <span class="dark-mustard-text">Summary </span>

1) Shows how to find CE in OLG + production 
2) When CE is not PO because of pecuniary inefficiency // $k* \neq k^{GR}$
3) How debt can be used to make CE PO by using govt policy 

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

## <span class="dark-mustard-text">Overview </span>

- OLG settings have several key features
    1. agents are finite-lived, but economy is infinite-lived
    2. agents are heterogeneous: young are different from old 
    3. environment is dynamic & general eqm
    4. ==markets are incomplete==
    5. competitive eqm generally not Pareto optimal
    6. a natural role for government policy to improve outcomes

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

## <span class="dark-mustard-text">A Growth Model </span>

- time discrete, $t = 1, 2, \ldots$
- at $t$, $N_t$ identical two-period-lived agents born
- endowed with 1 unit of labor in 1st period; nothing in 2nd period
- ==population evolves as $N_t = (1 + n)^t N_0$, $N_0$ given==
- preferences of generation $t$ are $u(c^y_t, c^o_{t+1})$
- $u(\cdot, \cdot)$ has usual properties plus:
    - $v(c^y, c^o) \equiv \frac{\partial u}{\partial c^y} / \frac{\partial u}{\partial c^o}$
    - $\lim_{c^y \to 0} v(\cdot) = \infty$ for $c^o > 0$
    - $\lim_{c^o \to 0} v(\cdot) = 0$ for $c^y > 0$
- old at initial date endowed with $K_0$
- consumption goods can be costlessly converted into capital
- ==capital chosen at $t-1$ is productive at $t$==
- capital does not depreciate
- representative firm has CRS technology $Y_t = F(K_t, N_t)$
- aggregate resource constraint:
    - $F(K_t, N_t) + K_t = K_{t+1} + N_t c^y_t + N_{t-1} c^o_t$
- convert to per capita: 
    - $k_t \equiv K_t/N_t$, $f(k_t) \equiv F(k_t, 1)$
    - $f(k_t) + k_t = (1 + n)k_{t+1} + c^y_t + \frac{c^o_t}{1 + n}$ (1)

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

## <span class="dark-mustard-text">Pareto Optimality </span>

- A Pareto optimal allocation is a sequence $\{c^y_t, c^o_t, k_{t+1}\}_{t=1}^{\infty}$ satisfying (1) such that no other allocation exists that also satisfies (1) with the property:
 
$\hat{c}^o_1 \geq c^o_1$, $u(\hat{c}^y_t, \hat{c}^o_{t+1}) \geq u(c^y_t, c^o_{t+1})$, $\forall t$ 

==with strict inequality in at least one instance.==

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

### <span class="dark-mustard-text">Social Planner's Steady State</span>

- Consider a steady state with $k_t = k$, $c^y_t = c^y$, $c^o_t = c^o$
- Social Planner solves:
    - $\max_{c^y, c^o, k} u(c^y, c^o)$ 
    - s.t. $f(k) - nk = c^y + \frac{c^o}{1 + n}$ (This is ARC)
- FOCs imply:
    - $\frac{u_1}{u_2} = 1 + n$;  $f'(k) = n$ (2)
- Note: ==Golden Rule== in rep-agent maxes $\tilde{c}$ in steady state:
    - $f(\tilde{k}) - n\tilde{k} = \tilde{c}$
    - $\frac{\partial \tilde{c}}{\partial \tilde{k}} = f'(\tilde{k}) - n = 0 \implies f'(k_{GR}) = n$

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

## <span class="dark-mustard-text">Competitive Equilibrium</span>

- What is the CE?
- Firm solves $\max_{K_t, N_t} F(K_t, N_t) - w_t N_t - r_t K_t$
- FOCs in per capita terms:  
    - $f'(k_t) = r_t$
    - $f(k_t) - k_t f'(k_t) = w_t$              (3)
- Young agents in generation $t$ solve:
    - $\max_{c^y_t, c^o_{t+1}, s_t} u(c^y_t, c^o_{t+1})$
    - $c^y_t = w_t - s_t$ ;  $c^o_{t+1} = (1 + r_{t+1})s_t$.    (4)
- FOCs imply:
    - $u_1[w_t - s_t, (1 + r_{t+1})s_t] = u_2[w_t - s_t, (1 + r_{t+1})s_t](1 + r_{t+1})$
    - $s_t = s(w_t, r_{t+1})$        (5)

### Definition:

A Competitive Equilibrium is sequences of quantities $\{k_{t+1}, s_t\}_{t=0}^{\infty}$ and prices $\{w_t, r_t\}_{t=0}^{\infty}$ where:

1. <span class="dark-mustard-text">consumers satisfy (5), taking prices as given </span>
2. <span class="dark-mustard-text">firms satisfy (3), taking prices as given </span>  
3. <span class="dark-mustard-text">markets clear for t = 0, 1, 2,....</span>

The CE solves:
- $k_{t+1}(1 + n) = s(w_t, r_t)$ 
- $k_{t+1}(1 + n) = s[f(k_t) - k_t f'(k_t), f'(k_{t+1})]$

This is a nonlinear difference equation in $k$ whose solution gives us $\{k_t\}_{t=0}^{\infty}$, which yields $r$ and $w$ from (3), $s$ from (5), and the $c$'s from (4).

### CE Example

$u(c^y, c^o) = \ln(c^y) + \beta \ln(c^o)$
$F(K, L) = \gamma K^{\alpha} L^{1-\alpha}$

- Young agents' problem:
    - $\max_{s_t} \{\ln(w_t - s_t) + \beta \ln[(1 + r_{t+1})s_t]\}$
    - Solution is $s_t = \frac{\beta}{1 + \beta} w_t$
- For the firm: 
    - $f(k) = \gamma k^{\alpha}$
    - $r_t = \gamma \alpha k_t^{\alpha-1}$
    - $w_t = (1 - \alpha) \gamma k_t^{\alpha}$

- Equilibrium condition (6) equates investment to saving:
    - $(1 + n)k_{t+1} = \frac{\beta}{1 + \beta} (1 - \alpha) \gamma k_t^{\alpha}$
- Steady state:
    - $k^* = \left[\frac{\beta \gamma (1 - \alpha)}{(1 + n)(1 + \beta)}\right]^{\frac{1}{1-\alpha}}$
    - $r^* = \frac{\alpha(1 + n)(1 + \beta)}{\beta(1 - \alpha)}$
    - $w^* = \gamma(1 - \alpha) \left[\frac{\beta \gamma (1 - \alpha)}{(1 + n)(1 + \beta)}\right]^{\frac{\alpha}{1-\alpha}}$
    - $c^y = \frac{w^*}{1 + \beta}$, $c^o = \frac{\beta}{1 + \beta} w^* (1 + r^*)$

Dynamics converge to $k^*$

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
### Pareto Optimality Revisited

- Is the CE Pareto optimal?
- Pareto optimal $k$ comes from (2):
    - $f'(k) = n \implies \tilde{k}_{GR} = \left(\frac{\alpha \gamma}{n}\right)^{\frac{1}{1-\alpha}} \neq k^*$ (CE capital)  
- Social planner can improve welfare over CE
    - PO sets $r = n$ (more generally, $r = n + \delta$)
- Cannot say if in CE $k$ is over- or under-accumulated $\implies$ no reason to expect it to be socially optimal
- CE not even Pareto efficient (i.e., no way to make one gen better off without making another worse off)

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

### Understanding Inefficiencies

- It can turn out that $r^* \lessgtr n$
    - When $r^* > n$, $k^* < k_{GR}$, so $c^* < c_{GR}$
        - to raise $k^*$, planner needs to get current gen to save more, making them worse off to benefit future gens
    - When $r^* < n$, $k^* > k_{GR}$, so reduced saving can increase consumption for every gen 
        - economy is dynamically inefficient
        - neoclassical growth model rules this out with transversality conditions
        - Start at steady state at $T$ with $k^* > k_{GR}$
            - change next period capital-labor by $-\Delta k$, $\Delta k \in (0, k^* - k_{GR})$  
            - then keep ratio at $k^* - \Delta k$
        - consumption is:
            - $\Delta c_T = (1 + n)\Delta k > 0$
            - $\Delta c_t = -\left[f'(k^* - \Delta k) - (1 + n)\right]\Delta k$, for $t > T$
        - increase in $c$ can be allocated equally across periods for each gen, raising utility $\implies$ Pareto improvement

- Source of inefficiency is not:
    - non-competitive markets
    - usual externalities
    - incomplete markets per se 
- ==It is "pecuniary externalities" - price effects of others' trading decisions on household utility==
    - wages of gen $t$ depend on capital of gen $t-1$
    - returns on saving of gen $t-1$ depend on capital of other members of $t-1$
    - usually pecuniary externalities are second-order
    - here choices of $t-1$ affect all future gens, so first-order effects
    - ==Current young save for old age \& more they save, lower is return on $k$, inducing them to save more== 
    - ==Could solve problem if there are alternative ways to provide consumption to the old ==

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

## <span class="dark-mustard-text">Government Policy</span>

(Govt introduces bonds and taxes here)

- $B_{t+1}$: one-period govt bonds issued at $t$
- $1 + r_{t+1}$: gross real return on consumption goods at $t+1$
- Bonds & capital yield same return (no arbitrage) 
- Assume $B_{t+1} = bN_t$ (per capita bonds constant)

- Govt flow identity: $B_{t+1} + T_t = (1 + r_t)B_t$
- Tax rule: $T_t = \tau_t N_t$ ($\tau_t$ is per capita taxes) // there were no taxes before 

- Young agents' problem:
    - $\max_{s_t} u[w_t - s_t - \tau_t, (1 + r_{t+1})s_t]$
    - Optimal savings is $s_t = s(w_t - \tau_t, r_{t+1})$
- Firms' problem unchanged 
- CE definition includes $\{\tau_t\}_{t=0}^{\infty}$ satisfying govt identity

- Combine tax & debt rules with budget identity:
    - $\tau_t = \frac{r_t - n}{1 + n} b$
    - Private saving can be held in $k$ or $b$, so market clearing is:
        - $k_{t+1}(1 + n) + b = s(w_t - \tau_t, r_{t+1})$
    - Substitute for prices & taxes:
        - $k_{t+1}(1 + n) + b = s\left[f(k_t) - k_t f'(k_t) - \frac{f'(k_t) - n}{1 + n} b, f'(k_{t+1})\right]$
- Solution for $k$ now a function of $b$, so steady state $k^*(b)$ solves:
    - $k^*(b)(1 + n) + b = s\left[f(k^*(b)) - k^*(b)f'(k^*(b)) - \frac{f'(k^*(b)) - n}{1 + n} b, f'(k^*(b))\right]$
- What is optimal level of debt? 
    - Answer: a $b_{GR}$ such that $k^*(b_{GR}) = k_{GR}$ (level of $b$ that induces CE to equal Golden Rule $k$)
    - Given $f'(k_{GR}) = n$, implies:
        - $b_{GR} = -k_{GR}(1 + n) + s(f(k_{GR}) - k_{GR} n, n)$
        
	    - $b^{GR} > 0 \implies$ transfers wealth from young to old
	    - $b^{GR} < 0 \implies$ transfers wealth from old to young


<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

## <span class="dark-mustard-text">Discussion</span>

- ==Ricardian equivalence fails to hold: debt financing matters because it directly affects capital accumulation, real interest rates, consumption, and utility==
- Can reinterpret this as social security: tax young and transfer resources to old
- Government is reducing or expanding total saving through variations in debt
- World real interest rates now low and expected to continue to decline
- Are we now in a dynamically inefficient equilibrium due to overaccumulation of capital?
- If so, model prescribes larger government borrowing[[OLG_fall]]
[[OLG+]]
