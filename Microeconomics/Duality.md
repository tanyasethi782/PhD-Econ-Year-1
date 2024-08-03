R/p b/w: 
* Hicksian Dd fn & Exp function 
* Hicksian and Walrasian function 
* Walrasian and indirect utility function 


---
## <span class = "teal-text">Hicksian Dd fn & Exp function </span>

e(p,u) = p. h(p, u)

1) Shephard's Lemma 
$h(p,u) = \frac{\partial e(p,u)}{\partial p}$
![[Pasted image 20240108184422.png]]
2) Substitution Matrix
![[Pasted image 20240109153944.png]]
Properties: 
	* Negative Semi-definite ([[Definiteness of the Substitution Matrix]]) 
		a matrix is negative semidefinite if, for any non-zero vector x, the product x′Ax is less than or equal to zero, where A is your matrix. Essentially, a negative semi-definite matrix indicates that the quadratic form it represents does not have any positive values. // Negative semi-definiteness means te function is concave as second order derivative would be negative so all diagonal entries would be negative.  
	* Symmetric (Mathematical Property)
	* $D_ph(p,u)p=0$
		* Implication: Every good has atleast one substitute. 
		* As $\frac{\partial h_l}{\partial p_l} \geq 0 \implies  \frac{\partial h_l}{\partial p_k} \leq 0$ (for atleast one k) for $D_ph(p,u)p=0$
	
![[Pasted image 20240623215507.png]]
___
## <span class = "teal-text">The Hicksian and the Walrasian Demand Functions   </span> 

1) Slutsky Equation. 

![[Note Nov 19, 2023.pdf]]


![[Pasted image 20240109220822.png]]

* Slutsky Substitution Matrix 

![[Pasted image 20240109223117.png]]

 Also need to look at Varian for the discrete case. Tested in the exams. 

Class Notes: 
![[Note Oct 23, 2023 (2).pdf]]

------
## <span class = "teal-text"> Walrasian and the indirect utility function</span>

1) Roy's Identity 
* The analogous for Shephard's lemma does not hold  -> Why?  <span class = "orange-text">The additional step of dividing by the wealth derivative of the indirect utility function in Roy's identity is necessary since the indirect utility function, unlike the expenditure function, has an ordinal interpretation: any strictly increasing transformation of the original utility function represents the same preferences while it's not true for x. </span>

* So, we normalize the derivative of v(p, w) wrt p by the marginal utility of wealth 
	
	$x_l(p,w) = - \frac{\partial v(p,w)}{\partial p} / \frac{\partial v(p,w)}{\partial w}$

Proof: 

Strategy: utility function --> use the expenditure function --> find the demand 

![[Pasted image 20240109002908.png]] 
----
Money Metric Utility Function 
Money Metric Indirect Utility Function 
