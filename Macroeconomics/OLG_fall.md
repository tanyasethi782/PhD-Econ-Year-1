
## 6 Overlapping Generations Model

### 6.1 A Pure Exchange OG Model

Consider an economy in discrete time $t = 1, 2, \ldots$ where in each period there are 2 types of agents: young and old. Each generation lives for 2 periods, while the economy lasts forever. We label each generation by the birth time period. Each generation $t$ has endowments in $t$ and $t+1$, $(e^t_t, e^t_{t+1})$. Correspondingly, generation $t$ consumes $(c^t_t, c^t_{t+1})$ in periods $t$ and $t+1$, correspondingly. 

Thus, in each time period $t$ there is an old generation with endowment $e^{t-1}_t$ and consumption $c^{t-1}_t$, and a young generation with endowment $e^t_t$ and consumption $c^t_t$ (see incidence matrix in table 1). In the first period, there is a generation of initially old agents with endowment $e^0_1$ and consumption $c^0_1$.

In some cases, we will consider a version of the model where initially old generation is endowed with some amount of outside money $m$. Cases with $m \geq 0$ are interpreted as flat money, and $m < 0$ may carry an interpretation of some debt that initially old borrowed in the past and now have to repay.

Agents derive utility from their consumption profiles according to the utility function
$$u^t(c) = U(c^t_t) + \beta U(c^t_{t+1}),$$
while the initially old generation gets the following utility
$$u^0(c) = U(c^0_1).$$
We will routinely assume that $U(\cdot)$ is strictly increasing, strictly concave and twice continuously differentiable.

#### Definitions

**Definition 16.** An allocation is consumption for initially old $c^0_1$ and a sequence of consumption allocations for generations $t \geq 1$, $(c^t_t, c^t_{t+1})^\infty_{t=1}$.

**Definition 17.** An allocation $c^0_1, (c^t_t, c^t_{t+1})^\infty_{t=1}$ is feasible if for all $t \geq 1$, 
$$c^{t-1}_t + c^t_t = e^{t-1}_t + e^t_t.$$

**Definition 18.** An allocation $c^0_1, (c^t_t, c^t_{t+1})^\infty_{t=1}$ is Pareto Optimal if it is feasible and there is no other feasible allocation $\hat{c}^0_1, (\hat{c}^t_t, \hat{c}^t_{t+1})^\infty_{t=1}$, such that
$$u^t(\hat{c}^t_t, \hat{c}^t_{t+1}) \geq u^t(c^t_t, c^t_{t+1})$$
$$u^0(\hat{c}^0_1) \geq u^0(c^0_1),$$
with at least one of inequalities being strict.

#### 6.1.1 Arrow-Debreu Equilibrium

**Definition 19.** An ADE for the OG model with money is an allocation $c^0_1, (c^t_t, c^t_{t+1})^\infty_{t=1}$ and the price system $\{p_t\}^\infty_{t=1}$, such that:

1. given $m$ and the $p_1$, $c^0_1$ must solve the problem of generation 0:
$$\max_{c^0_1} u^0(c^0_1)$$
$$p_1 c^0_1 \leq p_1 e^0_1 + m$$
$$c^0_1 \geq 0;$$

2. given the price system, $(c^t_t, c^t_{t+1})^\infty_{t=1}$ must solve generation's $t$ problem:  
$$\max_{c^t_t, c^t_{t+1}} U(c^t_t) + \beta U(c^t_{t+1})$$
$$p_t c^t_t + p_{t+1} c^t_{t+1} \leq p_t e^t_t + p_{t+1} e^t_{t+1}$$
$$c^t_t \geq 0, c^t_{t+1} \geq 0;$$

3. markets clear. For all $t \geq 1$ 
$$c^{t-1}_t + c^t_t = e^{t-1}_t + e^t_t.$$

**Remark:** Without outside money there will be no trade between generations. To see this, note that initially old will simply consume their endowment $e^0_1$ because they will be dead next period, and generation 1 will thus consume their endowment at time $t=1$. At time $t=2$, generation 1 will also simply consume their endowment $e^1_2$ since generation 2 will not give anything to them ($t=2$ is the last time period for generation 1). And so on. In other words, outside money allows to violate the budget constraint for initially old.

#### 6.1.2 Sequential Markets Equilibrium

**Definition 20.** A SME for the OG economy with money consists of allocations $c^0_1, (c^t_t, c^t_{t+1}, s^t_{t+1})^\infty_{t=1}$ and interest rates $\{r_{t+1}\}^\infty_{t=0}$, such that:  

1. given $r_1$, $c^0_1$ solves: 
$$\max_{c^0_1} u^0(c^0_1)$$
$$c^0_1 \leq e^0_1 + (1+r_1)m$$
$$c^0_1 \geq 0;$$

2. given the interest rate $r_{t+1}$, $(c^t_t, c^t_{t+1}, s^t_{t+1})$ must solve generation's $t$ problem:
$$\max_{c^t_t, c^t_{t+1}, s^t_{t+1}} U(c^t_t) + \beta U(c^t_{t+1})$$  
$$c^t_t + s^t_{t+1} \leq e^t_t$$
$$c^t_{t+1} \leq (1+r_{t+1})s^t_{t+1} + e^t_{t+1}$$
$$c^t_t \geq 0, c^t_{t+1} \geq 0;$$

3. markets clear. For all $t \geq 1$ 
$$c^{t-1}_t + c^t_t = e^{t-1}_t + e^t_t.$$

**Remark:** In case of an infinitely-lived consumer, we also added a No-Ponzi Game condition preventing the household from rolling over on debt. In case of a finitely-lived household this condition is redundant since whichever debt it is making at time $t$ needs to be repaid in $t+1$. This implicitly uses perfect enforceability of contracts.

#### 6.1.3 Equivalence between ADE and SME

**Theorem 10.** Let the allocation $\hat{c}^0_1, (\hat{c}^t_t, \hat{c}^t_{t+1})^\infty_{t=1}$ and the price system $\{p_t\}^\infty_{t=1}$ with $p_t > 0$ for all $t$ constitute an Arrow-Debreu equilibrium. Then there is a corresponding Sequential Market equilibrium with allocations $\tilde{c}^0_1, (\tilde{c}^t_t, \tilde{c}^t_{t+1}, \tilde{s}^t_{t+1})^\infty_{t=1}$ and interest rates $\{r_t\}^\infty_{t=1}$, such that
$$\hat{c}^t_t = \tilde{c}^t_t \text{ for all } t \geq 1$$  
$$\hat{c}^{t-1}_t = \tilde{c}^{t-1}_t \text{ for all } t \geq 1.$$

And the other way around, suppose $\tilde{c}^0_1, (\tilde{c}^t_t, \tilde{c}^t_{t+1}, \tilde{s}^t_{t+1})^\infty_{t=1}$ and interest rates $\{r_t\}^\infty_{t=1}$ constitute a Sequential Markets equilibrium with $r_t + 1 > 0$ for all $t$. Then there is an Arrow-Debreu equilibrium with allocations $\hat{c}^0_1, (\hat{c}^t_t, \hat{c}^t_{t+1})^\infty_{t=1}$ and the price system $\{p_t\}^\infty_{t=1}$, such that:
$$\tilde{c}^t_t = \hat{c}^t_t \text{ for all } t \geq 1$$  
$$\tilde{c}^{t-1}_t = \hat{c}^{t-1}_t \text{ for all } t \geq 1.$$

#### 6.1.4 Analysis using Offer Curves

Assuming $U(c) = \log c$, which is a strictly increasing function, we can drop non-negativity constraints from the generation $t$'s problem. The solution will be interior.
$$\max_{c^t_t, c^t_{t+1}} \log c^t_t + \beta \log c^t_{t+1}$$
$$p_t c^t_t + p_{t+1} c^t_{t+1} = p_t e^t_t + p_{t+1} e^t_{t+1}.$$

The system of first-order conditions is:
$$\frac{\partial L}{\partial c^t_t} = \frac{1}{c^t_t} - p_t \lambda = 0$$
$$\frac{\partial L}{\partial c^t_{t+1}} = \frac{\beta}{c^t_{t+1}} - p_{t+1}\lambda = 0.$$

These FOCs imply $c^t_{t+1} = c^t_t \beta \frac{p_t}{p_{t+1}}$. Next, divide both sides of the budget constraint by $p_t$ to get:
$$c^t_t + c^t_{t+1} \frac{p_{t+1}}{p_t} = e^t_t + e^t_{t+1} \frac{p_{t+1}}{p_t}.$$

Substituting the FOC:
$$c^t_t(1+\beta) = e^t_t + e^t_{t+1} \frac{p_{t+1}}{p_t}.$$

For initially old, normalizing the budget constraint by $p_t$ yields:
$$c^0_1 = e^0_1 + \frac{m}{p_1}.$$

**Remark:** Note that we cannot normalize the price system because it will change consumption of the initially old.  

**Definition 21.** Excess demand of consumer $i$ in an endowment economy is the difference between demand and endowment of consumer $i$.

#### 6.1.5 Equilibrium May Not Be Efficient

When we discussed economies where households are infinitely-lived, we were able to show that the First Welfare theorem holds: the equilibrium allocation is Pareto efficient. In OG models, however, this may not necessarily be the case. 

To show the potential failure of the FWT, it suffices to construct a feasible allocation which Pareto dominates the equilibrium one. For example, consider an OG model without money $m=0$ where the endowment stream is time-invariant $(e^t_t, e^t_{t+1}) = (2,1)$. As we have argued above, the equilibrium will be an autarky whereby agents consume their endowments, $(c^t_t, c^t_{t+1}) = (2,1)$. 

Consider another feasible allocation $(\tilde{c}^t_t, \tilde{c}^t_{t+1}) = (1.5, 1.5)$. Clearly, the initially old are strictly better off because
$$u^0(1.5) > u^0(1).$$
But all other generations are also better off in this alternative allocation, since:
$$u^t((2,1)) = \log 2 + \log 1 < \log \frac{9}{4} = u^t((1.5,1.5)).$$

### 6.2 OG Model with Production

#### 6.2.1 Sequential Markets Equilibrium

**Definition 23.** A Sequential Markets equilibrium for this economy is an allocation for the initially old, $(\hat{c}^0_1, \hat{l}^0_1)$, an allocation for generations $t \geq 1$, $\{\hat{c}^t_t, \hat{c}^t_{t+1}, \hat{l}^t_t, \hat{l}^t_{t+1}, \hat{k}^t_{t+1}, \hat{b}^t_{t+1}\}^\infty_{t=1}$, an allocation for firms, $\{\hat{y}_t, \hat{k}^f_t, \hat{l}^f_t\}^\infty_{t=1}$, and a price system $\{\hat{r}^k_t, \hat{w}_t, \hat{r}^b_t\}^\infty_{t=1}$, such that: 

1. given $(\hat{r}^k_1, \hat{r}^b_1, \hat{w}_1)$, $(\hat{c}^0_1, \hat{l}^0_1)$ solves:
$$\max u(c^0_1, l^0_1)$$
$$c^0_1 \leq \hat{w}_1 l^0_1 + (1-\delta+\hat{r}^k_1)\bar{k}_1 + (1+\hat{r}^b_1) m$$
$$0 \leq l^0_1 \leq \bar{l}_2;$$

2. given the prices, $\{\hat{c}^t_t, \hat{c}^t_{t+1}, \hat{l}^t_t, \hat{l}^t_{t+1}, \hat{k}^t_{t+1}, \hat{b}^t_{t+1}\}$ solves:
$$\max u(c^t_t,l^t_t) + \beta u(c^t_{t+1}, l^t_{t+1})$$
$$c^t_t + k^t_{t+1} + b^t_{t+1} \leq \hat{w}_t l^t_t$$ 
$$c^t_{t+1} \leq \hat{w}_{t+1} l^t_{t+1} + (1-\delta+\hat{r}^k_{t+1}) k^t_{t+1} + (1+\hat{r}^b_{t+1}) b^t_{t+1}$$ 
$$0 \leq l^t_t \leq \bar{l}_1, 0 \leq l^t_{t+1} \leq \bar{l}_2;$$

3. given prices, $\{\hat{y}_t\}^\infty_{t=1}$, $\{\hat{l}^f_t, \hat{k}^f_t\}$ solves 
** Not Complete 