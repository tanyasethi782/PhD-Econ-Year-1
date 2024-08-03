<span class="dark-mustard-text">**</span>

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
# <span class="dark-mustard-text"> Two-Period Exchange Economy Environment and Market Structure </span>

### The Environment

- Representative agent $i \in [0, 1]$
- Two time periods $t = 1, 2$
- Commodities
    - one perishable consumption good each period
    - endowments $Y_1$, $Y_2$ (no production)
- Preferences: linearly separable discounted utility
    - $U = u(C_1) + \beta u(C_2)$
    - $C_t$ is consumption in period $t$
    - $u(C_t)$ is period utility function, satisfies $u'(\cdot) > 0 > u''(\cdot)$ – positive but diminishing MU (more is better but at a decreasing rate)
    - Inada conditions guarantee interior solutions: $\lim_{c \to 0} u'(c) = \infty$, $\lim_{c \to \infty} u'(c) = 0$


<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

### Planner's Problem

- Having specified the environment allows us to solve the planner's problem
- But here this is a bit uninteresting
    - Just consume what you have: $Y_1 = C_1$, $Y_2 = C_2$


<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

### Market Structure

- Assume intertemporal market to trade $B_2$ units of discount bonds, i.e. bonds that cost $\frac{1}{1+r}$ in period 1 and repay 1 in period 2
    - → gross rate of return $R = (1 + r)$, net rate of return $r = R − 1$
- Budget constraints (BC) for periods 1 and 2:
    - BC1: $C_1 + \frac{B_2}{1 + r} = Y_1$
    - BC2: $C_2 = Y_2 + B_2$
- By eliminating $B_2$ we obtain the Intertemporal Budget Constraint (IBC): $C_1 + \frac{C_2}{1 + r} = Y_1 + \frac{Y_2}{1 + r}$
- Strategies: Agents maximize utility subject to IBC

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

## Partial Equilibrium

### Optimization

- Plug IBC into constrained problem to get unconstrained problem
    - $\max u(C_1) + \beta u(Y_2 + (1 + r)(Y_1 − C_1))$
- FOC: The Euler Equation
    - $u'(C_1) = \beta(1 + r)u'(C_2)$
- Interpretation – MU of eating more now equals MU of saving it at return $1 + r$ to eat tomorrow
- Another representation – price of discount bond $p_b$
    - $IMRS = \frac{\beta u'(C_2)}{u'(C_1)} = \frac{1}{1 + r} = p_b$
    - Intertemporal MRS equals ratio of MUs which equals relative price
- Implicit assumption – good 1 is numeraire, good 2 has a price of $\frac{1}{1+r}$

### Transversality Condition and No-Ponzi Condition

- Digression: What if we introduced the possibility of bond purchases $B_3$ in period 2 to repay in a (non-existing) period 3?
    1. each individual agent would find it suboptimal to buy – since the bonds will not repay within the horizon of the model; therefore: $B_3 \leq 0$
        - → this is an individual optimality condition that will, in infinite horizon models, correspond to the Transversality Condition (TVC)
    2. since nobody finds it optimal to purchase bonds, nobody will in equilibrium be able to sell bonds (i.e. borrow) in the last period; therefore: $B_3 \geq 0$
        - → this is a market-imposed constraint that will, in infinite horizon models, correspond to the so-called No Ponzi Condition
        - → together, the two conditions imply that $B_3 = 0$

### Steps to Solve the Model

Two Steps to Solve the Model

1. Partial equilibrium (PE) analysis: solve individual optimization problems taking prices as given
    - can be done graphically
    - and also analytically
2. General equilibrium (GE) analysis: aggregate individual choices and impose market clearing
    - to solve for equilibrium prices and allocations
    - again, this can be done graphically
    - and analytically

### Graphical Partial-Equilibrium (PE) Analysis

- Solid Lines in the Graph:
    - Indifference curves - ${(C_1, C_2) : u(C_1) + \beta u(C_2) = \bar{u}}$
        - moving up and to the right makes people happier (higher $\bar{u}$)
        - If $u(C) = \ln C$, then indifference curves are given by $C_1 C_2 = e^{\bar{u}}$ which are rectangular hyperbolas
    - Budget line and budget set
        - budget line: ${(C_1, C_2) : C_2 = Y_2 + (1 + r)(Y_1 − C_1)}$
        - budget set: area between origin and budget line (corresponding to weak inequality above)
    - Question: why can equilibrium not be at another point on the budget constraint?

## General Equilibrium

### General Equilibrium (GE) Analysis

- Equilibrium is where indifference curve is tangent on endowment bundle
- Slope of indifference curve corresponds to price $-\frac{1}{1+r}$
- Look for prices such that markets clear ($C_1 = Y_1$, $C_2 = Y_2$, $B_2 = 0$) while all agents optimize
    - $MRS = \frac{\beta u'(C_2)}{u'(C_1)} = \frac{1}{1 + r} = p_b$
    - → implies equilibrium price $p_b = \frac{1}{1+r} = \frac{\beta u'(Y_2)}{u'(Y_1)}$
- Why does market clearing require $B_2 = 0$?
    - there is no exogenous supply of bonds
    - representative consumer cannot sell bonds to herself

### Alternative Representation of Equilibrium

- Alternative: Diagram of Bond Market (PE)
- Alternative: General Equilibrium in Bond Market ($B_2 = 0$)

### Comparative Statics

- Observe the following comparative statics:
    - $\frac{dp_b}{dY_2} = \frac{\beta u''(Y_2)}{u'(Y_1)} < 0$
    - $\frac{dr}{dY_2} = \frac{dr}{dp_b}\frac{dp_b}{dY_2} > 0$
    - If $Y_2$ increases, the demand for bonds decreases - people wish to borrow more in period 1
    - This drives down the price of bonds in period 1, or equivalently drives up the interest rate
- Elasticity of Intertemporal Substitution (IES)
    - Definition of Elasticity: The elasticity of the marginal utility of consumption with respect to consumption $\sigma(C) = u'(C),C = -\frac{du'(C)}{dC}\frac{C}{u'(C)} = -\frac{u''(C)C}{u'(C)}$
    - Comparative Statics Using Elasticity of MU:
        - Consider the logarithm of the Euler equation $\log u'(C_1) = \log \beta(1 + r)u'(C_2)$
        - Taking total derivatives using the chain rule, $\frac{u''(C_1)}{u'(C_1)}dC_1 = d \log(1 + r) + \frac{u''(C_2)}{u'(C_2)}dC_2$
        - Using the definition of $\sigma$, $−\sigma(C_1)dC_1 = d \log(1 + r) − \sigma(C_2)dC_2$
- Iso-Elastic Utility
    - Isoelastic or constant-elasticity of substitution (CES) utility is defined:
        - for $\sigma \neq 1$: $u(C) = \frac{C^{1−\sigma} −1}{1−\sigma}$
        - for $\sigma = 1$: $u(C) = \log C$.
    - and has the property that $\sigma(C) = \sigma \forall C$
    - the expression on the previous slide then simplifies to $d \log(\frac{C_2}{C_1}) = \frac{1}{\sigma} d \log(1 + r)$
        - where $\frac{1}{\sigma}$ represents the intertemporal elasticity of substitution (IES), which is the inverse of the elasticity of marginal utility
    - Intuition: a high $\sigma$ (low IES) implies that $\frac{C_2}{C_1}$, and hence $B_2$, does not respond much to changes in $r$ (or $p_b$)
- Example Using Isoelastic Utility
    - Explicit GE solution for CES utility:
        - If $u(C) = \frac{C^{1−\sigma} −1}{1−\sigma}$, then the Euler equation is: $C_1^{-\sigma} = \beta(1 + r)C_2^{-\sigma}$ or: $C_2 = [\beta(1 + r)]^{\frac{1}{\sigma}}C_1$
        - using the intertemporal budget constraint, $C_1 = \frac{1}{1 + (1 + r)^{\frac{1}{\sigma}-1}\beta^{\frac{1}{\sigma}}}(Y_1 + \frac{Y_2}{1 + r})$

### Comparative Statics

- A change in $r$ has three effects
    1. Substitution Effect - Captured by $(1 + r)^{\frac{1}{\sigma}}$ in the denominator
        - As $r$ increases, substitute from $C_1$ into $C_2$
    2. Income Effect - Captured by $(1 + r)^{-1}$ in the denominator
        - As $r$ increases, earnings increase, making agents richer, thereby increasing both $C_1$ and $C_2$
    3. Wealth Effect - Captured by $\frac{Y_2}{1+r}$ in the numerator
        - As $r$ increases, the present value of $Y_2$ decreases

## Rational Expectations

### Expectations in Macroeconomics

- Role of expectations:
    - expectations are crucial when solving intertemporal problems
- Standard/simplest route: rational expectations
    - rational expectations means that agents have model-consistent, or "unbiased, on average" expectations
    - → they expect the economy to behave as modeled
    - first proposed by Muth (1961)
    - popularized by Lucas in the mid 1960s
    - note: rational expectations have nothing to do with the expectations operator in stochastic models
        - they only mean that agents' understanding of the model lets them predict future processes (including all future probabilities) correctly

### Evaluating Rational Expectations

- Discussion of Rational Expectations:
    - Are RE a good model assumption to describe the world? → it all depends
        - good e.g. for day-to-day market movements
        - bad e.g. for unknowable uncertainties (eg. bubbles, panics)
- Alternative:
    - Adaptive Expectations
        - people extrapolate the past
        - empirically quite relevant in many applications

## Markets with Uncertainty

### Economies with Uncertainty

Include Uncertainty in Model Environment

- To capture uncertainty in an economic model, we enrich the environment:
    - Probability Space $(S, M, \Pi)$ `a la Kolmogorov
        - $S$ - Sample space
        - $M$ - Sigma algebra
        - $\Pi$ - Probability measure over events in $M$
    - Assume state of nature $s \in S$ realized at date 2
        - e.g. $S = {L, H}$ or $S = {sunny, rainy, cloudy}$
    - Events are subsets of the state space $E \subseteq S$ s.t. $E \in M$
    - Define a countably additive probability measure $\Pi(E) \in [0, 1]$
        - For discrete states, denote $\pi(s) = \pi_s = \Pi({s}) = probability$ of $s \in S$
- Recall: random variables in this economy are functions of the state $s$
    - e.g. $Y_2(s) = Y^s_2$ is the output in state $s$ of period 2
    - → note: interpret goods in different states of nature as different goods

### Preferences over Uncertain Outcomes

- Expected Utility
    - $U = u(C_1) + \beta E_\Pi[u(C_2)]$
    - expectation usually taken over objective probability measure
- But: agents may also have a subjective probability measure different from $\Pi(E)$, for example:
    - agents may have probability measure $P(E)$ reflecting greater pessimism
    - or over-optimism $O(E)$ regarding the future
- Expectations operator $E_\Pi[\cdot]$:
    - if state space $S$ is discrete/countable, $E_\Pi[f(s)] = \sum_{s \in S} \pi(s)f(s)$
    - in the general case, $E_\Pi[f(s)] = \int_{s \in S} f(s)d\Pi(s)$ using Lebesgue integral
    - for simplicity of notation, we will generally omit the superscript indicating the probability measure and just write $E[\cdot]$

### Risk

- Risk Aversion
    - Uncertainty makes it important to consider attitudes towards risk.
        - Definition (Risk Aversion 1): A utility function $u(\cdot)$ is risk-averse if $E[u(C^s)] < u(E[C^s])$ for any non-degenerate random variable $C^s$
        - By Jensen's inequality, this definition is equivalent to
            - Definition (Risk Aversion 2): A utility function $u(\cdot)$ is risk-averse if it is strictly concave.
- Measures of Risk Aversion
    - Risk Compensation: captures how much agent needs to be paid to make up for risk
        - For risky payoff $z$ at deterministic consumption level $y$, we define the risk compensation $\rho(y, z)$ s.t. $E[u(y + z)] = u(y − \rho + z)$
            - $\rho \equiv$ risk compensation (premium)
            - $y − \rho \equiv$ certainty equivalent
        - Note that $\rho$ is a scalar, and not an RV like $z$.
    - Arrow-Pratt Coefficient of Relative Risk Aversion
        - $R(C) = -\frac{u''(C)}{u'(C)} \cdot C = MU(C)$
    - Utility functions with constant relative risk aversion (CRRA):
        - $u(C) = \frac{C^{1−\sigma}}{1−\sigma}$ for $\sigma \neq 1$ or $u(C) = \log C$ for $\sigma = 1$
        - Exercise: show that these functions satisfy $R(C) = \sigma = constant$ $\forall C$

### Market Structure

- Market Structure under Uncertainty
    - With uncertainty, the precise market structure takes on great importance
    - Several possibilities:
        1. Complete markets: market allows agents to trade every