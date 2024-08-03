The reason why restricting $\phi \geq 0$ implies that the eigenvalue for equation (1) lies in the interval $[0, \infty)$ has to do with the structure of the equation and the properties of eigenvalues.

Recall that equation (1) is:

$\phi x_t = z_t + E_t x_{t+1}$

Assuming rational expectations and rearranging the equation, we get:

$E_t x_{t+1} - \phi x_t = -z_t$

Now, let's consider the general form of a linear first-order difference equation:

$E_t y_{t+1} - \lambda y_t = 0$

Here, $\lambda$ is the eigenvalue (or the characteristic root) of the equation. The stability of the solution depends on the value of $\lambda$.

Comparing this general form to our rearranged equation, we can see that $\phi$ in equation (1) plays the same role as $\lambda$ in the general form. Therefore, $\phi$ is the eigenvalue of equation (1).

Now, the properties of eigenvalues state that:
1. If $|\lambda| < 1$, the system has a stable root, and the solution is convergent.
2. If $|\lambda| > 1$, the system has an unstable root, and the solution is explosive.
3. If $|\lambda| = 1$, the system has a unit root, and the solution is non-stationary.

==When we restrict $\phi \geq 0$, we are essentially saying that the eigenvalue of equation (1) can take any non-negative real value.== This includes values greater than or equal to 0 and less than 1 (which would lead to a stable solution), exactly equal to 1 (which would lead to a unit root), and greater than 1 (which would lead to an explosive solution).

Therefore, restricting $\phi \geq 0$ implies that the eigenvalue of equation (1) can lie anywhere in the interval $[0, \infty)$, which includes both stable and unstable regions.



******
In the model we've been discussing:

$\phi x_t = z_t + E_t x_{t+1}$

When we rearrange the equation to match the general form, we get:

$E_t x_{t+1} - \phi x_t = -z_t$

Here, $\phi$ takes the place of $\lambda$ in the general form. The stability conditions for this specific model are:

1. If $|\phi| < 1$, the system has a stable root.
2. If $|\phi| > 1$, the system has an unstable root.
3. If $|\phi| = 1$, the system has a unit root.

However, the determinacy of the solution depends not only on the stability of the root but also on the presence of a transversality condition or a boundary condition that rules out explosive paths.

When $0 \leq \phi < 1$, the system has a stable root, but there are multiple solutions (indeterminacy) because any arbitrary stochastic process ${\xi_t}$ that satisfies $E_t \xi_{t+1} = 0$ can be a solution.

When $\phi > 1$, the system has an unstable root. However, if we impose a transversality condition or a boundary condition that rules out explosive paths, we can find a unique, determinate solution by solving the model forward. This is because the forward solution:

$x_t = \frac{1}{\phi} \sum_{k=0}^\infty \left(\frac{1}{\phi}\right)^k E_t z_{t+k}$

converges when $\phi > 1$, as the weight on future expected values of $z_t$ decreases exponentially.

So, while the system has an unstable root when $\phi > 1$, we can still find a unique, convergent solution by imposing a boundary condition that excludes explosive paths. This is why, in the context of this model, we find a determinate solution when $\phi > 1$.