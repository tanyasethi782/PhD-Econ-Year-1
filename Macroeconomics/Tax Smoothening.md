

## We follow (Barro, 1979)
* Key Assumption of this approach is that debt is always fully repaid
* The government is smoothening taxes while trying to fit stochastic $g_t$ by using debt 





Setup:
- Representative consumer endowed with $Y$ units of goods each period
- Tax distortions reduce the endowment
  - $\Phi(T_t)$: strictly increasing in $T_t$, convex, $\Phi(0) = 0$, $\Phi'(0) > 0$
  - Consumer's income: $Y_t = Y - \Phi(T_t)$
- Government spending $G_t$ is exogenous
- Utility: $U(C) = \ln(C)$

Social Planner's Problem:
$$\max_{C_t, A_t} E_0 \sum_{t=0}^\infty \beta^t \ln(C_t)$$
$$\text{s.t. } C_t + A_t \leq Y - \Phi(T_t) + (1+r)A_{t-1}, \quad \forall t$$
$$\lim_{t \to \infty} \beta^t E_t[U'(C_{t+1})(1+r)A_t] = 0 \text{ (TVC)}$$
$$A_{-1}, G_t \text{ given}$$

FOCs:
$$\frac{1}{C_t} = \lambda_t$$
$$\lambda_t = \beta E_t[\lambda_{t+1}(1+r)]$$
$$\lambda_t = \beta(1+r)E_t[\lambda_{t+1}]$$
$$\lambda_t = \frac{1+r}{1+\rho} E_t[\lambda_{t+1}], \quad \text{where } \beta \equiv \frac{1}{1+\rho}$$

Goods Market Clearing:
$$C_t + G_t = Y - \Phi(T_t)$$

Welfare Function:
$$U(C_t) = \ln(Y - G_t - \Phi(T_t))$$

Government Budget Identity:
$$\beta^t b_{t+1} = (1+r)b_t + G_t - T_t$$

Government's Problem:
$$\max_{T_t, b_t} E_0 \sum_{t=0}^\infty \beta^t \ln(Y - G_t - \Phi(T_t))$$
$$\text{s.t. } b_{t+1}(1+r) = b_t + G_t - T_t, \quad \forall t$$
$$\lim_{t \to \infty} \beta^t b_{t+1} = 0 \text{ (TVC)}$$

FOCs:
$$\frac{\Phi'(T_t)}{Y - G_t - \Phi(T_t)} = \mu_t$$
$$\mu_t = E_t[\mu_{t+1}]$$

- MB of higher $T_t$: $\mu_t$
- MC of higher $T_t$: $\frac{\Phi'(T_t)}{Y - G_t - \Phi(T_t)}$
- Smooth tax distortions over time

### Example

Assume:
$$G_t = \begin{cases}
  \bar{G}^H & \text{if } t = 0 \\
  \bar{G}^L & \text{if } t \geq 1
\end{cases}$$
$$E_t[T_{t+j}] = \bar{T}, \quad \forall j \geq 1$$
$$b_{t+1}(1+r) = b_t + \bar{G}^H - T_0$$
$$b_{t+1}(1+r) = b_t + \bar{G}^L - \bar{T}, \quad \forall t \geq 1$$

After imposing TVC:
$$\lim_{t \to \infty} E_t[\beta^t b_{t+1}] = 0$$

Optimal $T_t$'s:
$$T_t = \frac{r}{1+r}b_t + \frac{1}{1+r}E_t\left[\sum_{j=0}^\infty \beta^j G_{t+j}\right]$$

- Pay the bondholders: $\frac{r}{1+r}b_t$
- Cover the PV of spending: $\frac{1}{1+r}E_t\left[\sum_{j=0}^\infty \beta^j G_{t+j}\right]$

Permanent spending:
$$\bar{G} \equiv (1-\beta)E_t\left[\sum_{j=0}^\infty \beta^j G_{t+j}\right]$$

Solving for $b_t$:
$$b_t = \bar{G}^H - T_0 + \frac{1}{1+r}E_t[b_{t+1}]$$
$$b_t = \bar{G}^H - T_0 + \frac{1}{1+r}(\bar{G}^L - \bar{T}) + \beta E_t[b_{t+1}]$$

## Transversality and Uniqueness

Consider the difference equation:
$$\frac{1}{C_t} = \beta E_t\left[\frac{1+r}{C_{t+1}}\right]$$

Define:
$$Z_t \equiv \beta^t \frac{U'(C_t)}{1+r} K_t$$

Then:
$$Z_t = \beta E_t[Z_{t+1}]$$

Iterate forward:
$$Z_t = \beta^j E_t[Z_{t+j}], \quad \forall j \geq 1$$

Assume:
$$\lim_{j \to \infty} \beta^j E_t[Z_{t+j}] = 0 \text{ (TVC)}$$

Then:
$$Z_t = 0$$

This pins down a unique solution.
