---
aliases:
  - February 2024 Notes
tags:
  - Macroeconomics
---

## Steady State
- Golden Rule: $\max_c \frac{c}{1-\beta}$ 
    - $f(K)/n$
        - Divide this by n (per capita terms)
    - $f(K)/n - \delta K$
    - Young agent:
        - $\max U = \sum_{t=0}^\infty \beta^t \frac{c_t^{1-\theta}}{1-\theta}$
        - s.t. $c_t + s_t = w_t$
        - $c_{t+1} = r_{t+1} s_t$ 
- FOC's imply:
    - $\frac{1}{c_t} = \beta r_{t+1} \frac{1}{c_{t+1}}$
    - $\frac{w_t - s_t}{s_t} = r_{t+1}$
    - $s_t = \frac{w_t}{1+r_{t+1}}$
    - saving = $f(K_t) - c_t$

## Competitive Equilibrium
- $K_{t+1} = s_t$, so $w_t = r_t = 0$ (mkt clearing)
- The CE solves:
    - $K_{t+1} = f(K_t) - n c_t$
    - $w_t = f(K_t) - K_t f'(K_t)$  
    - $r_t = f'(K_t)$
- Non-linear diff eq in k
- $U(c_t, c_{t+1}) = \frac{c_t^{1-\theta}}{1-\theta} + \beta \frac{c_{t+1}^{1-\theta}}{1-\theta}$
- FOC: $y = r k + (1-\delta)k$

## Young's Problem
- $s_t = \frac{w_t}{1+r_{t+1}}$ (savings only depend on $\beta$, not MRS)

## Firm (per capita)
- $E = \frac{s_2K^\alpha}{w = (1-\alpha)K^\alpha}$
- $n=1 \implies k=K$
- If $\alpha = \frac{1}{3}, \frac{5}{9} K_t = S_t = \frac{K_{t+1}}{n}$
- $\therefore K_t \nearrow$ soon because of savings reinvested until $s_t = \delta K_t$

## Optimal k* from Golden Rule
- $f'(k^*)=n(1+\rho)$
- CE capital (and consumption) is lower
- GP can improve welfare over the competitive equilibrium
- PO sets $r=n$ (treats rents with depreciation)
- Cannot say if CE $\overset{?}{\underset{>}{<}} k^*$ (over or under accumulates K)
- but can say $c_r^{PO} > c_r^{CE}$

## It can turn out that:
- $r < n$ when $n > k f'(k)$
- Max $C = c^{AR}$ (SS consM)

## To raise $k^*$, SP needs to get the young to save more
- then current gen is worse off to make future gens better off
- but what about current gen when old?

## When $r > n$, $k < k^{GR}$ (reduced saving can make all generations better off)
- $\because$ people live only 2 periods. Can't happen in neoclassical because of TVC (cannot overaccumulate)

## Sources of Inefficiency
- It is pecuniary externalities (price-related effects of the trading decisions of others on the utility of the HH)
- Agents of gen t don't face wages determined by capital decisions of gen t-1 (does not happen in rep agent model)
- Agents of gen t-1 receive a return on savings determined by other members of gen t-1 (this is same as rep agent model)
- Usually pecuniary externalities = second order & small
- Here gen t-1 choices affect all future gens = first order effects
- Current young save for old age, more they save, the lower the return (increases saving more)

## Introducing Govt Bonds
- Bet = one period govt bonds at t 
- $r_{t+1}$ = gross real return
- No arbitrage: $k_t$ & $B_t$ have same return
- Assume $B_{t+1} = \phi B_t$ (per capita bonds are constant)
- GBC: $B_{t+1} = r_{t+1} B_t + T_t$
- Tax rule: $T_t = \phi B_t - (1-\phi)r_t B_t$

## Young's Problem
- $s_t = \frac{w_t - T_t}{1+r_{t+1}}$

## Optimal Saving
- $s_t = \frac{w_t}{1+r_{t+1}} - \frac{T_t}{1+r_{t+1}}$

## Tax rule, debt rule, GBC
- How does this come?
    - $T_t = (r_t - \rho) B_t$

## Derive by here: GBC
- Mkt Clearing: $K_{t+1} = f(K_t) - n c_t + \phi B_t$
    - $c_t = \frac{f(K_t) - s_t}{n} - \frac{(1-\phi)B_t}{n}$
    - $\frac{K_{t+1}}{n} = \frac{1}{n} [f(K_t) - c_t + \phi B_t]$
    - $K_{t+1} = (1-\phi)B_t + f(K_t) - c_t$
    - SOE for k is a fn of b
    - ss: $\bar{K} = \frac{b}{1-\phi}$
        - $\bar{K} = \frac{\phi \bar{b}}{1-\phi} + f(\bar{K}) - \frac{f(\bar{K})}{n} - \frac{(1-\phi)\bar{b}}{n}$
        - $(1-\phi)\bar{b} = \phi \bar{b} -\delta \bar{K}$ 
        - $\phi = \frac{\delta \bar{K}}{\bar{b} + \delta \bar{K}} \implies \bar{b} = f'(\bar{K}) - (1+n)\delta$

## What is the optimal level of debt?
- It is $\bar{b} = \frac{f'(\bar{K})}{n} - (1+\rho)$
    - since $f'(\bar{K}) = n(1+\rho)$
- $\therefore \bar{b} = \frac{\rho \delta \bar{K}}{n(1+\rho)}$
    - $\bar{b} > 0$ transfers wealth from young to old
    - $\bar{b} < 0$ transfers wealth from old to young