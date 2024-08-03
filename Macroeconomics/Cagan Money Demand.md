
## Money in the Utility Function

Setup:
- Non-interest bearing fiat currency (money) with no intrinsic value
- $M_t$: nominal money balances
- $P_t$: price level
- $m_t \equiv \frac{M_t}{P_t}$: real money balances
- $\mu_t \equiv \frac{M_t}{M_{t-1}}$: exogenous stochastic money growth
- Ignore real interest rate

Equilibrium:
$$\frac{m_t}{m_{t-1}} = \frac{M_t/P_t}{M_{t-1}/P_{t-1}} = \frac{\mu_t P_{t-1}}{P_t}$$

This is a difference equation. Demand for money is a forward-looking decision. $m_t$ depends on expected inflation.

Iterate forward:
$$\frac{M_t}{P_t} = \beta E_t\left[\frac{M_{t+1}}{P_{t+1}}\right]$$
$$\frac{1}{P_t} = \beta E_t\left[\frac{\mu_{t+1}}{P_{t+1}}\right]$$

Assume $\lim_{j \to \infty} \beta^j E_t\left[\frac{M_{t+j}}{P_{t+j}}\right] = 0$ (TVC).

Then:
$$\frac{1}{P_t} = \sum_{j=1}^\infty \beta^j E_t\left[\frac{\mu_{t+j}}{M_{t+j}}\right]$$

### Example: Two-State Markov Chain

Suppose $\mu_t$ follows a two-state Markov chain with transition matrix:
$$P = \begin{bmatrix}
  p_{11} & 1-p_{11} \\
  1-p_{22} & p_{22}
\end{bmatrix}$$

Assume $P$ is irreducible and aperiodic.

Then:
$$E_t\left[\frac{\mu_{t+j}}{\mu_{t+j-1}}\right] = \sum_{k \in \{\text{low}, \text{high}\}} \frac{\mu_k}{\mu_{t+j-1}} P^j_{kt}$$

where $P^j$ is the $j$-step transition matrix and $\mu_k$ is the money growth rate in state $k$.

Letting $j \to \infty$:
$$\lim_{j \to \infty} E_t\left[\frac{\mu_{t+j}}{\mu_{t+j-1}}\right] = \sum_{k \in \{\text{low}, \text{high}\}} \mu_k P^\infty_{k}$$

$P^\infty$ exists because $P$ is irreducible and aperiodic. Its largest eigenvalue is 1.

#### Numerical Example

Assume:
- $\mu_\text{low} = 1$, $\mu_\text{high} = 1.04$
- Low $\mu$ regime is both more common and more persistent
  - 50% chance of leaving high $\mu$ regime in each period

Then:
$$P = \begin{bmatrix}
  0.8333 & 0.1667 \\
  0.5 & 0.5
\end{bmatrix}$$

$$P^\infty = \begin{bmatrix}
  0.7143 & 0.2857 \\
  0.7143 & 0.2857
\end{bmatrix}$$

Therefore:
$$\lim_{j \to \infty} E_t\left[\frac{\mu_{t+j}}{\mu_{t+j-1}}\right] = 1 \cdot 0.7143 + 1.04 \cdot 0.2857 = 1.0114$$

### Extension: Regime Switching with Noise

Modify the process:
$$\mu_t = \bar{\mu}_t(1 + \varepsilon_t), \quad \varepsilon_t \overset{iid}{\sim} N(0, \sigma^2)$$

Assume agents observe $\mu_t$ but neither the state $\bar{\mu}_t$ nor $\varepsilon_t$.

Use Bayesian updating with PDFs. If there is no overlap between the distributions of $\mu_t$ in the two states, you can confidently infer the state. Otherwise, it's tougher.