---
tags:
  - Macroeconomics
---
<span class="dark-mustard-text">**</span>

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
## <span class="dark-mustard-text">Background</span>

- When solving difference equations, analysts frequently invoke a "transversality" condition to justify setting a limit to zero
- Less frequently, analysts connect that condition to some explicit optimization problem
- This note makes the connection explicit
    1. Specify model
    2. Obtain necessary & sufficient conditions for optimum
    3. ==Derive difference equation whose solution yields optimal decision rule==
    4. ==Show convergence of difference equation ensured by transversality==

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
## <span class="dark-mustard-text"> Simplest Growth Model </span> 

- Assume log preferences, inelastic labor, complete depreciation of capital, Cobb-Douglas production
    - None are necessary: just allow closed-form solution
- Solve social planner's problem $$\max_{{C_t,K_t}} E_1\sum_{t=1}^{\infty} \beta^t \ln(C_t)$$ $$C_t + K_t = A_tK_{t-1}^{\alpha} \equiv Y_t \qquad (1)$$
- Comments
    - ${A_t}$ random technology process
    - note timing of capital: $K_t$ chosen at $t$, used at $t+1$
    - $E_t$ formed based on all variables dated $t$ and earlier
    - $K_0 > 0$ given, $0 < \alpha \leq 1$, $0 < \beta < 1$
    - equation (1) is the aggregate resource constraint

## Optimality Conditions

- FOCs imply $$\frac{1}{C_t} = \beta E_t \left[\frac{\alpha A_{t+1}K_t^{\alpha-1}}{C_{t+1}} \right] \qquad (2)$$
- Transversality is $\lambda_t K_t \rightarrow 0$, so from FOC: 
 $$\lim_{T\to\infty} \beta^T E_t U'(C_{t+T})K_{t+T} = 0 \qquad (3)$$
- (2) combines FOCs for $C_t$ & $K_t$
- ==(3) is the "transversality condition"==
    - ==in the limit, the expected discounted utility value of capital is zero==
    - ==ensures that at an optimum, agent isn't over-accumulating capital (i.e., not over-saving)==
    - ==one of the necessary & sufficient conditions for an optimum==

## Solution

- Solve by hand
- Rewrite (2) as $$\frac{K_t}{C_t} = \alpha\beta E_t \left[\frac{Y_{t+1}}{C_{t+1}}\right] = \alpha\beta E_t \left[\frac{C_{t+1}+K_{t+1}}{C_{t+1}}\right]$$
- ==Apply the magic of adding 1 to both sides to obtain difference equation in $z_t \equiv (C_t+K_t)/C_t$== $$\frac{C_t+K_t}{C_t} = 1 + \alpha\beta E_t \left[\frac{C_{t+1}+K_{t+1}}{C_{t+1}}\right]$$ $$z_t = 1 + \alpha\beta E_t z_{t+1}$$
- Because $0 < \alpha\beta < 1$, solve forward $$z_t = \sum_{j=0}^{T-1} (\alpha\beta)^j + (\alpha\beta)^T E_t z_{t+T} \qquad (4)$$

## Solutions

- ==(4) is not the solution because $E_t z_{t+T}$ is not determined==
    - ==Actually, it is many solutions==
- To obtain (4) we used the Euler equation, (2), and the resource constraint, (1)
    - This tells us the set of solutions for $z$ (the inverse of the saving rate) that are candidate equilibrium decision rules
- ==The solution would be unique if as we take the limit we get== $$\lim_{T\to\infty} (\alpha\beta)^T E_t z_{t+T} = 0 \qquad (5)$$
- Notice that we haven't used transversality, (3)
    - This means that (4) may admit as possible solutions $z_t$ processes that fail to satisfy (3)

## Imposing Transversality

- Evaluate the limit in (5) 
-$\begin{align*} \lim_{T\to\infty} (\alpha\beta)^T E_t z_{t+T} &= \lim_{T\to\infty} (\alpha\beta)^T E_t \left[1 + \frac{K_{t+1}}{C_{t+1}}\right]\ &= \lim_{T\to\infty} (\alpha\beta)^T E_t U'(C_{t+T})K_{t+T} \qquad (6) \end{align*}$
==Where does 1 go?==
- Since $0 < \alpha \leq 1$, $\alpha\beta \leq \beta$, (6) $\implies$ (3), and $$\lim_{T\to\infty} (\alpha\beta)^T E_t z_{t+T} = 0$$
^ ==Imposing transervasility condition makes this zero and hence leads to a unique solution!!!==
- The unique equilibrium saving function and decision rules are $$\frac{C_t+K_t}{C_t} = \frac{1}{1-\alpha\beta} \qquad (7)$$ $$C_t = (1-\alpha\beta)A_tk_{t-1}^{\alpha} \qquad (8)$$ $$K_t = \alpha\beta A_t K_{t-1}^{\alpha} \qquad (9)$$

## The Economics of Transversality

- The Euler equation says that at an optimum, there can be no intertemporal substitution of consumption & savings that raises utility
- Take the FOC for $K_t$ $$U'(C_t) = \beta E_t U'(C_{t+1})f'(K_t) \qquad (10)$$
- (10) says
    - to exchange one unit of $C_t$ for $K_t$ costs the marginal utility
    - at $t+1$, get in expectation, $f'(K_t)$ more goods that when converted to consumption yield utility value $U'(C_{t+1})$, discounted by $\beta$ to time $t$
    - any consumption/capital sequences that satisfy (10) are candidate equilibria
    - notice the swap at $t$ is reserved at $t+1$
    - ==The Euler equation is silent about swaps at $t$ that are never reversed==

## The Economics of Transversality

- Transversality is about permanent swaps of $C$ for $K$
- Consider (3) $$\lim_{T\to\infty} \beta^T E_t U'(C_{t+T})K_{t+T} = 0 \qquad (3)$$
- At $t$, swap 1 unit of $C_t$ for 1 unit of $K_t$
    - Hold that additional unit of $K$ for the infinite future
    - What is the value of that permanent swap at time $t$?
    - ==Transversality says that value must be zero==
    - ==This ensures that at an optimum, there are no permanent swaps of consumption for saving that yield higher utility==
- Because transversality is about the "long run," some economists believe it can never bite in practice
    - Maybe, but this isn't any different from many other features of optimizing behavior
    - I just think of it as saying that people don't want to over-accumulate assets

## Abuse of "Transversality"

- It is commonplace for economists to invoke "transversality" in situations where it does not apply
- True transversality conditions emerge from optimization
    - They say that choices that do not satisfy the condition are sub-optimal
    - That justifies eliminating as equilibria some sequences that satisfy Euler equations, which can deliver uniqueness
- It is not true that anytime you face a difference equation, there is a valid transversality condition that delivers convergence
- Also notice that (3) holds only in expectation
    - it needn't hold for all possible realizations
    - that is, $E_t U'(C_{t+T})K_{t+T} \neq U'(C_{t+T})K_{t+T}$ in general


Other Sources: [[Transversality Conditions]]