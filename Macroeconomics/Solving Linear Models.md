
<span class="dark-mustard-text">**</span>
<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>
Tools: 
[[Statistical stationarity]]
[[Difference Equation; Eigenvalues]]
[[Root Counting]]
<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>


## <span class="dark-mustard-text">Overview</span>

- In rational expectations models, indeterminacy of equilibrium is ubiquitous
- Indeterminacy takes multiple forms:
	1. multiple steady state equilibria 
	2. "loose" initial condition—many equilibrium paths that converge to a unique steady state equilibrium
	3. "sunspot" equilibrium that may introduce extraneous volatility
- By construction, linear models do not have multiple steady states
- We focus on linear (or linearized) models and forms (2) and (3)

## The Simplest Example

- Start with a univariate example
- Take the system to be:

$\phi x_t = z_t + E_t x_{t+1}, \phi \geq 0$ (1)
$z_t = \rho z_{t-1} + \varepsilon_t, 0 \leq \rho < 1$ (2)

where $x_t$ is an endogenous variable, $z_t$ is a stationary exogenous variable, $\varepsilon_t$ has finite variance

- (1) and (2) hold for $t = 1, 2, \dots$ with $z_0$ arbitrary 
- If (1) comes from an Euler equation, agents' optimal choices begin in $t=1$, so $E_1 x_2$ is the first expectation
- There appears to be indeterminacy:
	- three "unknowns"—$x_t$, $z_t$, $E_t x_{t+1}$  
	- two equations—(1) and (2)
- Resolving this indeterminacy requires an additional restriction—the essence of solving linear rational expectations models

<div style="border-bottom: 2px solid #00FFFF; margin: 10px 0;"></div>

## <span class="dark-mustard-text"> Conventional Solution Method </span> 

- Solutions to (1) take the general form:

$x_t = \phi x_{t-1} - z_{t-1} + \xi_t$, for $t = 1, 2, \dots$ (3)

where $\xi_t$ is a stochastic process that satisfies $E_t \xi_{t+1} = 0$

- Confirm that (3) solves (1)
- When an arbitrary $\xi_t$ process is consistent with equilibrium, there is a "sunspot" 
	- because the ${\xi_t}$ process is arbitrary, each process that satisfies $E_t \xi_{t+1}$ generates a different equilibrium process for $\{x_t\}$
	- this is the third form of indeterminacy
- ==We have restricted $\phi \geq 0$, but this means the eigenvalue for (1) lies in the interval $[0, \infty)$==  
(More at [[Difference Equation; Eigenvalues]])
- Now we consider the two cases:
	1. determinacy: $\phi > 1$
	2. indeterminacy: $0 \leq \phi < 1$

### Conventional Solution Method: Determinacy 
 <span class="dark-mustard-text">Suppose that $\phi > 1$</span>

<div style="border-bottom: 2px solid #11BBBB; margin: 10px 0;"></div>

- If we solve (1) "backward" we obtain:

$E_t x_{t+k} = \phi^k x_t - z_t \sum_{i=1}^k \phi^{k-i} \rho^{i-1}$

- If the shock is identically zero, $z_t \equiv 0$:

$\lim_{k \to \infty} E_t x_{t+k} = \lim_{k \to \infty} \phi^k x_t \to \infty$

So the solution is unbounded. 
- With no further structure, we cannot rule out such solutions as equilibria
	- if there is a transversality condition that rules out explosive $\{x_t\}$ processes, we have an economic reason to exclude those solutions
	- ==for now, we set this point aside to focus on bounded solutions==


<div style="border-bottom: 2px solid #11BBBB; margin: 10px 0;"></div>

- When $\phi > 1$, the "forward" solution is:

$x_t = \frac{1}{\phi} \sum_{i=0}^k \left(\frac{1}{\phi}\right)^i E_t z_{t+1} + \left(\frac{1}{\phi}\right)^k E_t x_{t+k}$

- Take the limit as $k \to \infty$ and second term disappears: 

$x_t = \frac{1}{\phi} \sum_{k=0}^\infty \left(\frac{1}{\phi}\right)^k E_t z_{t+k}$
$= \frac{1}{\phi} \sum_{k=0}^\infty \left(\frac{\rho}{\phi}\right)^k z_t$  
$= \frac{1}{\phi - \rho} z_t$, for $t = 1, 2, \dots$ (4)

- Substitute (4) into (3) for $x_t$ & $x_{t-1}$ to solve for $\xi_t$:

$\xi_t = \frac{1}{\phi - \rho} (z_t - \rho z_{t-1}) = \frac{1}{\phi - \rho} \varepsilon_t$, for $t = 1,2, \dots$ (5)

- (5) maps the fundamental shock, $\varepsilon_t$, uniquely into $\xi_t$ 
- ==when $\phi > 1$, only one process for $\{\xi_t\}$ is a solution to (1) & (4) is the unique bounded solution==




<div style="border-bottom: 2px solid #11BBBB; margin: 10px 0;"></div>
### <span class="dark-mustard-text">Conventional Solution Method: Indeterminacy</span>

- Suppose that $\phi < 1$  
- (3) describes the full set of bounded solutions to (1)
- Multiple solutions stem from two sources:
	1. solution for $x_1$ depends on both $z_0$ and $x_0$
		- ==$z_0$ is exogenous and can be arbitrarily given==
		- ==$x_0$ is not determined by the model ("loose initial condition")== 
		- ==each value of $x_0$ implies different path of $\{x_t\}$, even if $\xi_t \equiv 0$==
	2. any process for $\xi_t$ that satisfies $E_t \xi_{t+1} = 0$ is a solution
		- variance of $\xi_t$ is free, though bounded
		- each $var(\xi_t) \implies$ different stochastic process for $\{x_t\}$
- There is a double infinity of solutions to (1) when $0 \leq \phi < 1$ ❓
- Aside: indeterminacy may or may not produce more volatile solutions—$var(\xi_t) = 0$ is also a solution

<span class="dark-mustard-text">// Why did we not try to solve this forward or backward?</span>  


In comparison: 
when $\phi > 1$, both sources of indeterminacy disappear:

1. The initial condition $x_0$ is no longer relevant for the solution.
2. The stochastic process ${\xi_t}$ is uniquely determined by the fundamental shock ${\varepsilon_t}$.


<div style="border-bottom: 2px solid #11BBBB; margin: 10px 0;"></div>

## Minimum State Variable 

- Also called "guess and verify"
- Determine the state of the economy for the model:

$\phi x_t = z_t + E_t x_{t+1}$ (1)
$z_t = \rho z_{t-1} + \varepsilon_t$ (2) 

- Minimum state is $z_t$
- model is linear, so assume solution linear 
- guess solution: 
$x_t = a + b z_t$ (6)
- solve for $(a,b)$ such that guessed solution satisfies the model

### Steps
1. Use guess, (6), to compute $E_t x_{t+1} = a + b \rho z_t$
2. Insert guess for $x_t$ & $E_t x_{t+1}$ in (1) to yield:
	$\phi(a + bz_t) = z_t + a + b \rho z_t$
3. Equate coefficients on constant (1) & $z_t$ to get:  
	$\phi a = a$
	$\phi b = 1 + b \rho$
4. Solve for $(a,b)$:
	$a = 0$, when $\phi > 0$ ; <span class="dark-mustard-text">What if $\phi$ =1? </span>
	$b = \frac{1}{\phi - \rho}$
5. Solution is $x_t = \frac{1}{\phi - \rho} z_t$, as in (4)
6. ==Can say nothing about determinacy==


<div style="border-bottom: 2px solid #11BBBB; margin: 10px 0;"></div>

## Sims' Method

- gensys designed to generalize & automate solution methods
	- ==generalize by moving beyond "root counting" to check spanning conditions== // <span class="dark-mustard-text">how do we do this in the conventional approach? </span> 
	- automate by creating code to quickly solve & report existence/uniqueness
- Sketch of algorithm:
	1. ==replace expectations with realizations − forecast errors==
	2. put linear system in canonical (1st-order) form
	3. compute Jordan decomposition to obtain eigenvalues & eigenvectors
	4. check spanning conditions: existence & uniqueness
	5. suppress "unstable" roots
	6. derive mapping from fundamentals to forecast errors
	7. derive equilibrium (when unique)
- Apply procedure to univariate example

### Specify the System
- Notation:
	- $y_{t+1}$ vector of all endogenous & exogenous variables
	- $\varepsilon_{t+1}$ vector of fundamental (exogenous) shocks  
	- $\eta_{t+1} = x_{t+1} - E_t x_{t+1}$, one-step-ahead forecast error in endogenous variables
	- $C$ vector of constant terms (if any)
- System is:

$\Gamma_0 y_{t+1} = \Gamma_1 y_t + C + \Psi \varepsilon_{t+1} + \Pi \eta_{t+1}$, for $t=1,2,\dots$ (7)

- Timing in (7) important:
	- model in (1) & (2) operates $t=1$ onward
	- agents make initial choices at $t=1$, form initial expectations $E_1 x_2$  
	- we are solving for $\{x_t, E_t x_{t+1}\}$ for $t=1,2,\dots$

### The Algorithm
<span class="dark-mustard-text">// Why do we have both error term and forecast error? </span>
- Rewrite (1) as:
$x_{t+1} = \phi x_t - z_t + \eta_{t+1}$ (8)

- Define $y_t = (x_t, z_t)'$, so (1) & (2) in canonical form (7) is:

$\begin{pmatrix} 1 & 0\\\ 0 & 1 \end{pmatrix} \begin{pmatrix} x_{t+1} \\\ z_{t+1} \end{pmatrix} = \begin{pmatrix} \phi & -1\\\ 0 & \rho \end{pmatrix} \begin{pmatrix} x_t\\\ z_t \end{pmatrix} + \begin{pmatrix} 0\\\ 1\end{pmatrix} \varepsilon_{t+1} + \begin{pmatrix} 1\\\ 0\end{pmatrix} \eta_{t+1}$ (9) 

- In this model, $\Gamma_0 = I$, so multiplying through by its inverse yields:

$y_{t+1} = \Gamma y_t + C + \Psi \varepsilon_{t+1} + \Pi \eta_{t+1}$, for $t=1,2,\dots$ (10)

where $\Gamma = \Gamma_0^{-1} \Gamma_1 = \begin{pmatrix} \phi & -1\\\ 0 & \rho  \end{pmatrix}$

- Note: $\Gamma_0$ need not be invertible because gensys employs [[generalized inverses]]

- Apply Jordan decomposition to transition matrix $\Gamma$:

$\Gamma = P \Lambda P^{-1}$

where $\Lambda$ has the eigenvalues of $\Gamma$ along the diagonal:  
$\Lambda = \begin{pmatrix} \phi & 0\\\ 0 & \rho\end{pmatrix}$

$P$ and $P^{-1}$ are the matrices of right and left eigenvectors

- Eigenvectors are calculated as:

$P = \begin{pmatrix} 1 & \frac{1}{\phi-\rho}\\\ 0 & 1\end{pmatrix} \quad P^{-1} = \begin{pmatrix} 1 & -\frac{1}{\phi-\rho}\\\ 0 & 1\end{pmatrix}$ (11)

- Use (11) in (9) & premultiply by $P^{-1}$ to define the linear combination:

$w_{t+1} \equiv P^{-1} y_{t+1} = \Lambda w_t + P^{-1} C + P^{-1} (\Psi \varepsilon_{t+1} + \Pi \eta_{t+1})$ (12)

By focusing on solving system (12), we now are solving for these linear combinations of the original variables:  
$w_{1,t+1} = x_{t+1} - \frac{1}{\phi-\rho} z_{t+1}$  
$w_{2,t+1} = z_{t+1}$

The model's simplicity makes the second element of the $w$ vector exactly equal to the exogenous process, $z$.

- gensys allows for non-homogeneous growth rate restrictions
	- They take the form of linear combinations of variables, $\alpha_i y_t$ for $i=1,2,\dots,m$, that have bounded growth rates, with possibly different bounds for each $i$, to impose the restrictions:
	
	$E_s[\alpha_i y_t \zeta_i^{-t}] \to 0$ as $t \to \infty$  
	
	for all $i$ and $s$ with $\zeta_i > 1$
	- Jordan decomposition isolates components of system with distinct exponential growth rates
	- We exploit this to break the dynamics in the system into unrelated components

- $\Lambda$ has block-diagonal structure with typical block:

$w_{jt} = \begin{pmatrix} \lambda_j & 1 & 0 & \dots & 0\\\ 0 & \lambda_j & 1 & \dots & 0\\\ 0 & 0 & \ddots & \ddots & \vdots\\\ \vdots & \vdots & \ddots & \ddots & 1\\\ 0 & \dots & \dots & 0 & \lambda_j\end{pmatrix} w_{jt-1} + P_{j\cdot}C + P_{j\cdot} (\Psi \varepsilon_t + \Pi \eta_t)$ (13)

where $P_{j\cdot}$ are the rows of $P^{-1}$ in the $j$th block of (12) and $\lambda_j$ represents the eigenvalues associated with that $j$th block.

- In the absence of repeated roots, the matrix of $\lambda_j$'s in (13) is simply the scalar $\lambda_j$, so:

$w_{jt} = \lambda_j w_{jt-1} + P_{j\cdot} C + P_{j\cdot} (\Psi \varepsilon_t + \Pi \eta_t)$

- In deterministic steady state, $\varepsilon_t = \eta_t \equiv 0$, so if $\lambda_j \neq 1$, then the $j$th block of (12) has the deterministic steady state solution:

$w_{jt} = [I - \Lambda_j]^{-1} P_{j\cdot} C$ (14)

where $\Lambda_j$ is the Jordan block in (13).

- If for any $j$, $|\lambda_j| > 1$, then $E_s[w_{jt+s}]$ grows in absolute value at rate $|\lambda_j|^t$ as $t \to \infty$ for any solution other than that in (14)
- Consider the $k$th restriction on growth:

$E_s[\alpha_k y_t] \zeta_k^{-t} = \alpha_k P E_s[w_t] \zeta_k^{-t}$
$= \alpha_k P \left[ \Lambda^{t-s} (w_s - (I-\Lambda)^{-1} P^{-1} C) + (I-\Lambda)^{-1} P^{-1} C \right] \zeta_k^{

