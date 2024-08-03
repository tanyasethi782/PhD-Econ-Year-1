![[Slides_Optimization.pdf]]



the substitution matrix is an actual mathematical matrix that captures the substitution effects between different goods. Specifically, it's a matrix of second partial derivatives of the demand functions with respect to prices. 

<span class = "orange-text">**So, if you have a demand function for each good, this matrix shows how the demand for each good changes as the price of every good changes.**</span>

The reason why it's negative semidefinite relates to the properties of consumer preferences and the law of demand. <span class = "orange-text">In simple terms, a matrix is negative semidefinite if, for any non-zero vector x, the product x′Ax is less than or equal to zero, where A is your matrix. Essentially, a negative semi-definite matrix indicates that the quadratic form it represents does not have any positive values.</span>


If the Hessian $D^2f_x*$ is a negative definite matrix, then x* is a strict interior local max of f.
<span class = "red-text"> Its a minimization problem wrt x and not p, so it's fine. </span>


MWG: Since e(p,u) is a twice continuously differentiable concave function (see [[Concavity of expenditure function]]), it has a symmetric and negative semidefinite Hessian (second derivative) matrix. 


![[Pasted image 20240109153944.png]]

It implies $\frac{\partial h_i}{\partial p_i}< 0$ for all i. 

Why is the substitution matrix negative semidefinite? 

By the law of compensated demand: $dp.dh(p,u)\leq0$ (total change in the price * total change in the commodity demanded)
As $dh(p,u) = D_ph(p,u)dp$ (Total change in demand is change in demand per unit change in price * total change in price)

$\implies$ $dp.D_ph(p,u)dp \leq 0$
$\implies$ The matrix $D_ph(p,u)$ is negative semidefinite. 


See [[Partial & total derivatives]]






