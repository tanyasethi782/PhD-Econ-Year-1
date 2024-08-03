

## <span class="dark-mustard-text"> Security Market Economy</span>

### <span class="dark-mustard-text"> Environment and Market Structure</span>
A Security Market Economy
1. Environment: build on stochastic two-period setting from earlier with two small modifications:
   - $i = \{1, \ldots, N\}$ agents indexed by $i$
   - $S$ (finite) states of nature
2. Market Structure: our main focus today  
3. Equilibrium: adjusted for changes in market structure

### <span class="dark-mustard-text">### Securities</span>
Security market structure:
- Securities $j \in \{1, 2, \ldots, J\}$
- Securities are defined by their return $x^j \in \mathbb{R}^S$, which lists the payoff of security $j$ in each state $s$: $x^j = (x_{j1}, \ldots x_{jS})$
- Payoff matrix stacks all the payoff vectors vertically:

$$
X_{J \times S} = \begin{bmatrix}
x^1 \\
x^2 \\
\vdots \\
x^J
\end{bmatrix}
$$

- A portfolio $h \in \mathbb{R}^J$ describes an agent's holdings of the $J$ securities
- Payoff of portfolio is $z = h_{1 \times J} X_{J \times S} = \sum_{j=1}^J h_j x^j \in \mathbb{R}^S$

### <span class="dark-mustard-text">### Prices and Returns</span>
- Security prices: $p = (p_1, p_2, \ldots, p_J)$
- Price of portfolio: $p \cdot h = \sum_{j=1}^J p_j h_j$ (inner product)
- Gross return of security $j$: $r^j_{1 \times S} = \frac{x^j}{p_j} = \left(\frac{x_{j1}}{p_j}, \frac{x_{j2}}{p_j}, \ldots, \frac{x_{jS}}{p_j}\right)$

### <span class="dark-mustard-text">### Types of Securities</span>
Security = tradable financial asset
Examples:
- Bond - debt that can be traded
- Equity - ownership share of firm that pays dividends 
- Asset-based security (ABS) - security whose value depends on the value of a bundle of assets
- Option - right to buy/sell in the future at a fixed price
- Futures - agreement to buy or sell in the future at a fixed price
- Swap - exchanges risky payment for safe payment (offloads risk)

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

## <span class="dark-mustard-text">## Asset Span and Completeness</span>

### <span class="dark-mustard-text">### Asset Span</span>
Asset span $\mathcal{M}$ of a security economy = set of payoffs that can be obtained using the available securities = row space of $X$:

$$
\mathcal{M} = \{z \in \mathbb{R}^S : z = hX \text{ for some } h \in \mathbb{R}^J\}
$$

- Markets complete $\iff \mathcal{M} = \mathbb{R}^S$
- Markets incomplete $\iff \mathcal{M} \subsetneq \mathbb{R}^S$

Proposition: Markets are complete iff $rank(X) = S$.
- Market completeness means that all values in $\mathbb{R}^S$ are reachable
- This means we need at least $S$ securities.
- $J > S$ is a possible case for this – if $S$ of the $J$ securities are linearly independent

### <span class="dark-mustard-text">### Market Completeness</span>
Proposition: Markets are complete iff $rank(X) = S$.

Proof:
- $\implies$ If $rank(X) = S$, $\exists S$ linearly independent row vectors of length $S$ in $X$. Then, they span $\mathbb{R}^S$ (form a basis for it). Hence, markets are complete.
- $\impliedby$ If markets are complete, the row vectors in $X$ span $\mathbb{R}^S$. Then, pick out the linearly independent ones. This gives us a basis for $\mathbb{R}^S$. Then, we get that $rank(X) = S$.

Proof: $\mathcal{M} = \mathbb{R}^S$ iff $z = hX$ has a solution $\forall z \in \mathbb{R}^S$, i.e. $h = zX^{-1}$ (right inverse exists), which is equivalent to market completeness.

### <span class="dark-mustard-text">### Redundant Securities</span>
- Security $j$ is redundant if its payoffs $x^j$ can be replicated as a portfolio of the other securities, i.e. $\exists h$ s.t. $h_j = 0$ with $hX = x^j$
- A security that is not linearly independent of the other securities
- If $J > S$ then some securities must be redundant

Proposition: There are no redundant securities iff $rank(X) = J$.

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

## <span class="dark-mustard-text">## Optimization and Equilibrium</span>

### <span class="dark-mustard-text">### Optimization</span>
Strategy of each agent $i$:

$$
\max_{C_1^i, C_2^{is}, h^i} u(C_1^i) + \beta E [u(C_2^i)]
$$

s.t. 
$$

C_1^i + p \cdot h^i &= Y_1^i \\
C_2^{is} &= Y_2^{is} + \sum_{j=1}^J h_j^i x_j^s \quad \forall s, \text{ or equiv. } C_2^i_{1 \times S} = Y_2^i_{1 \times S} + h^i_{1 \times J} X_{J \times S}
$$

FOC ($h_j^i$): $p_j u'(C_1^i) = \beta \sum_{s \in S} \pi_s u'(C_2^{is}) x_j^s \quad \forall j$
or: $p_j = E [M^{is} x_j^s]$ where $M^{is} = \frac{\beta u'(C_2^{is})}{u'(C_1^i)}$ (stochastic discount factor)

### <span class="dark-mustard-text">### Equilibrium</span>

#### <u>Security Market Equilibrium)</u>:
An equilibrium in the security markets economy is a set of allocations $(C_1^i, C_2^i, h^i)$ and prices $(p)$ such that
- all individuals optimize, and
- markets clear: $\sum_i h^i = 0$ (security markets clear), $\sum_i C_1^i = \sum_i Y_1^i$, and $\sum_i C_2^i = \sum_i Y_2^i$ (goods markets clear)

#### <u>Law of One Price, LOOP)</u>: 
If $hX = h'X$, $p \cdot h = p \cdot h'$. 
(This is referring to the transpose of the H matrix - ==I don't understand this==)
- Note that this holds trivially if there are no redundant securities ($hX = h'X$ requires $h = h'$).

### <span class="dark-mustard-text">### Arrow Securities</span>
Arrow Securities (or State Claims):
- $e^s = (0, 0, \ldots, 1, \ldots, 0)$ is an Arrow security - ==a security that returns 1 unit of consumption in state $s$ and nothing in any other state==
- Denote cost of Arrow security $e^s$ by state price $q_s$
- If LOOP holds and markets are complete:
  - Well-defined $q_s$ for every state $s$
  - The vector $q \equiv (q_1, q_2, \ldots, q_S)$ is a payoff pricing functional 
  - $q: \mathbb{R}^S \to \mathbb{R}$ map stochastic payoff vectors into the (scalar) price space
  - For any $z \in \mathbb{R}^S$, $q \cdot z \equiv$ price of payoff $z$

### <span class="dark-mustard-text">### Optimization Problem in Payoff Space</span>
We can then express the optimization problem of agent $i$ as directly choosing a payoff vector $z^i$ (rather than a portfolio $h^i$ of securities):

$$
\max_{C_1^i, C_2^i, z^i \in \mathcal{M}} u(C_1^i) + \beta E [u(C_2^{is})]
$$

s.t. 
$$
\begin{align*}
C_1^i + q \cdot z^i &= Y_1^i \\
C_2^i &= Y_2^i + z^i
\end{align*}
$$

FOC ($z_s^i$): $q_s = \frac{\pi_s \beta u'(C_2^{is})}{u'(C_1^i)} =: \pi_s M^{is}$ 
... State prices equal the probability-weighted MRS $\pi_s M^{is}$ for each agent $i$ // ==where is the pi coming from?== 

$\implies q$ is frequently called "pricing kernel" and is unique under complete markets.

Note: $p_j = q \cdot x^j = \sum_{s \in S} q_s X_{js} \quad \forall j$ or $p = qX'$

### <span class="dark-mustard-text">### Fundamental Theorem of Finance!!</span>
Definition: An arbitrage is a portfolio with positive payoffs but zero price.
- Small arbitrage opportunities exist in practice, but they go away once engaged in.

Theorem (Fundamental Theorem of Finance): $q \gg 0$ is strictly positive (i.e. $q_s > 0 \forall s$) iff there is no arbitrage.

Proof:
Under complete markets, $p = Xq$. Then, $q = Lp$, where $L$ is the left inverse of $X$.
Note that $q \gg 0 \implies p \gg 0 \implies$ no arbitrage.
On the other hand, no arbitrage $\implies p \gg 0 \implies q \gg 0$.

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>


## <span class="dark-mustard-text">## Risk</span>

### <span class="dark-mustard-text">### Risk-neutral probabilities</span>
Let $\iota = (1, 1, \ldots, 1)$ be a risk-free bond
Then, $q \cdot \iota = \sum_s q_s$ is price of a risk-free bond
The risk-free return is then $\bar{r} = \frac{1}{q \cdot \iota} = \frac{1}{\sum_s q_s}$ // Question: why is iota (return) in ==denominator==? 

Definition (Risk Neutral Probabilities): $\pi_s^* = \bar{r}q_s = \frac{q_s}{\sum_s q_s}$
- Note that $\pi_s^*$ are non-negative and sum up to 1
- $\implies$ Use $\pi_s^*$ to construct a probability measure $\Pi^*(\{s\}) = \pi_s^*$
- This measure differs from the objective probability measure $\Pi$ because it reflects the market value of individual states of nature

### <span class="dark-mustard-text">### Risk-neutral probability space</span>
Definition (Risk-Neutral Probability Space):
The triple $(S, \mathcal{B}, \Pi^*)$ forms a probability space that we call the risk-neutral probability space (or Q-space) 
- This differs from the objective probability space (P-space)

The probability measure $\Pi^*$ and the associated expectations operator $E^*[\cdot]$ allow us to express:
- $q \cdot z = \frac{E^*[z]}{\bar{r}}$, $p_j = \frac{E^*[x^j]}{\bar{r}}$, $\bar{r} = E^*[r^j]$, $\forall j$

Example: Consider $S = \{L, H\}$ with $\pi_L = \pi_H = \frac{1}{2}$
Assume $C_2^L < C_2^H$: then, $q_L > q_H$, implying that $\pi_L^* > \frac{1}{2} > \pi_H^*$

### <span class="dark-mustard-text">### Risk Aversion</span>
Definition (Risk Aversion): A utility function $u(\cdot)$ is risk-averse if $E[u(C^s)] < u(E[C^s])$ for any non-degenerate random variable $C^s$
- By Jensen's inequality, this definition is equivalent to
Definition (Risk Aversion): A utility function $u(\cdot)$ is risk-averse if it is strictly concave.

<span class="dark-mustard-text">### Measures of Risk Aversion</span>
- Risk Compensation: For risky payoff $z$ at deterministic consumption level $y$, we define the risk compensation $\rho(y, z)$ s.t. $E[u(y + z)] = u(y - \rho + z)$ 
  - $\rho \equiv$ risk compensation (premium)
  - $y - \rho \equiv$ certainty equivalent 
  - Note that $\rho$ is a scalar, and not an RV like $z$.
- Arrow-Pratt Coefficient of Relative Risk Aversion: $R(C) = -\frac{u''(C)}{u'(C)} \cdot C = MU(C)$
- Utility functions with constant relative risk aversion (CRRA): $u(C) = \frac{C^{1-\sigma}}{1-\sigma}$ for $\sigma \neq 1$ or $u(C) = \log C$ for $\sigma = 1$
  - Exercise: show that these functions satisfy $R(C) = \sigma = constant \ \forall C$ 

<span class="dark-mustard-text">## The Equity Premium Puzzle</span>

<span class="dark-mustard-text">### The Sharpe Ratio</span>
From the agent's optimality condition
$E[u'(C_2^s)(r_j^s - \bar{r})] = 0$
$\implies \rho_{u', r_j - \bar{r}} = \frac{Cov(u'(C_2^s), (r_j^s - \bar{r}))}{\sigma(u'(C_2^s)) \sigma(r_j^s - \bar{r})}$

Since $|\rho| \leq 1$, 
$$
\sigma(u'(C_2^s)) \geq \frac{E[u'(C_2^s)] E[r_j^s - \bar{r}]}{\sigma(r_j^s)}
$$

Using $E[u'(C_2^s)] = \frac{u'(C_1)}{\beta \bar{r}}$,
$$
\sigma\left(\frac{\beta u'(C_2^s)}{u'(C_1)}\right) \geq \frac{1}{\bar{r}} \cdot \frac{|E[r_j^s] - \bar{r}|}{\sigma(r_j^s)}, \quad \forall j
$$
std dev of MRS $\geq$ Sharpe ratio

<span class="dark-must