Certainly! Let's replace the `<div>` tags with `<span>` tags and see if that works better. Here's the updated transcription:

<span class="dark-mustard-text">**Econ 8010 Maxim Engers**</span>  
<span class="dark-mustard-text">**Lecture 16**</span>

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">**Common Value Auction Example**</span>

- Simple Example: 2 bidders. 
- Private signals $t_i$ iid ~ $U[0,1]$.
- Value of object $t_1 + t_2$ same to both.
- Now, the higher type bidder doesn't value the object more but is just more optimistic: 
	- i.e. has a higher expectation of the value
- We look for a symmetric BNE in which both bidders use the same strictly increasing bid function $B$.
	- We can ignore ties: In equilibrium, their probability is 0.

<span class="blue-box">
This example is quite special. We could, in general, consider non-independent signals and the common value a more general function of the signals, but finding the equilibrium is harder. In solving our example, <b>additivity</b> and <b>independence</b> are what is crucial. They will allow us to use some of the same tricks we used in solving for symmetric equilibria in the IPV model, for different auction formats.
</span>

<span class="dark-mustard-text">**BNE of 1st Price CV Example**</span>

- Pick bidder $i$ of type $t$.
- Rival of type $t'$ bids $B(t')$
- $i$ chooses $b$ to maximize $i$'s expected payoff:
	$\pi(t, b) = Prob[i wins]\{t + E[t'| i wins] – b\}$
	$= Prob[B(t') < b]\{t + E[t'| B(t') < b] – b\}$.
- $i$'s equilibrium expected utility/payoff as a function of $i$'s type $t$ is:
	$u(t) = \max_b \pi(t, b) = \pi(t, B(t))$.
- Envelope theorem trick: 
	$u'(t) = \frac{\partial \pi}{\partial t}|_{b=B(t)} = F(t) = t$ in uniform case.
- Also $u(0) = 0$. (why?)
	<span class="yellow-box">
	Answer: In equilibrium, type 0 has 0 chance of winning and 0 chance of paying anything.
	</span>

Thus, 
$u(t) = \frac{1}{2} t^2 = \pi(t, B(t))$
$= Prob[B(t') < B(t)]\{t + E[t' | B(t') < B(t)] – B(t)\}$  
$= Prob[t' < t]\{t + E[t'| t' < t] – B(t)\}$
$= t[t + \frac{t}{2} – B(t)]$

Thus $B(t) = t$.

Next, we check this is sufficient for an equilibrium.

<span class="dark-mustard-text">**Sufficiency of Solution**</span>

- Suppose your rival uses $B(t') = \frac{t'}{2}$. 
- You will never bid an amount $b$ more than 1. Why?
	
	Bidding 1 gives the same probability of winning (1) at lower cost. Recall
$\pi(t, b) = Prob[B(t') < b]\{t + E[t' | B(t') < b] – b\}$
	$= Prob[ t' < b]\{t + E[t' | t' < b] – b\}$
	$= b(t + \frac{b}{2} – b)$
	$= b(t –\frac{b}{2})$
	quadratic, maximized at $b = t$.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">**CV Example: More General Auctions**</span>

More generally, suppose that the auction equilibrium satisfies the following 2 conditions:
1. both bidders use the same strictly increasing bid function $B$, and 
2. type 0 has expected payment of 0, i.e. $e(0) = 0$.

Use mechanism-design approach: Suppose bidder $i$ of type $t$ chooses to emulate type $s$, so that $i$'s bid will be $B(s)$, and let $e(s)$ denote $i$'s expected payment.   

#Ques: Why do we have emulation here? 

$i$'s expected payoff, if $i$'s type is $t$ and $i$ bids as a type $s$ would, is:
$\pi(s, t) = Prob[B(t') < B(s)]\{t + E[t' | B(t') < B(s)]\} – e(s)$
$= Prob[t' < s]\{t + E[t'| t' < s]\} – e(s)$

- Equilibrium expected payoff, $u(t) = \pi(t, t)$ 
- Envelope theorem says $u'(t) = \frac{\partial \pi}{\partial t}|_{s=t} = F(t) = t$ 
- Also $u(0) = 0$. (why?) 
	<span class="yellow-box">
	Answer: type 0 has 0 chance of winning in equilibrium and has expected payment of 0.
	</span>

Thus $u(t) = \frac{1}{2} t^2 = \pi(t, t)$
$= Prob[t' < t]\{t + E[t' | t' < t]\} – e(t)$ 
$= t(t + \frac{t}{2}) – e(t)$

Thus $e(t) = t^2$
#Ques: how are we replacing s with t here? 

==Thus, in our example, all BNE in which both bidders use the same strictly increasing bid function, and $e(0)=0$ are payoff-equivalent and revenue-equivalent.==

<span class="dark-mustard-text">**Could we just have applied the Revenue Equivalence Theorem (or its corollary) to get this result?**</span>

No. 

One of the assumptions of the Revenue Equivalence Theorem is that there are **Independent Private Values**: the theorem does not apply to the example we are considering.

Nevertheless, as we have just shown, some of the results extend.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">**CV Example: Solving for Equilibrium bid functions**</span>

**All-Pay**: $B(t) = e(t) = t^2$ 
(Check sufficiency as an exercise).

**1st price**: 
(We already solved this above, but notice how the $e(t)$ function easily gives the necessary condition determining $B(t)$)

$t^2 = e(t) = F(t)B(t) = tB(t)$

So, $B(t) = t$

**2nd price**: $t^2 = e(t) = F(t)E[B(t') | t' < t]$
- $F(t)$ is the probability that $i$ wins (and thus the probability that $i$ pays anything) 
- $E[B(t') | t' < t]$ is the expected amount $i$ pays if $i$ wins.

To calculate this, we need the distribution function of $i$'s rival's type, $t'$, conditional on $t'$ being less than $t$.

<span class="dark-mustard-text">**The conditional distribution**</span>

Let $G$ be the cumulative distribution function (cdf) of this conditional random variable. 

So, $G(x) = Prob(t' ≤ x | t' < t )$ is the probability that $t' ≤ x$ conditional on $t' < t$.

Recall $F$ is the cdf of the unconditional distribution of $t'$. 

Suppose $F(t) > 0$. For any $x < t$,

#Ques: Why do we take $x$ < $t$? 

$G(x) = Prob(t' ≤ x$ and $t' < t) / Prob(t' < t)$ (Why?... 
<span class="yellow-box">
Answer: Conditional Probability Formula
</span>

$= Prob(t' ≤ x) / Prob(t' < t )$ (Why?..
<span class="yellow-box">
Answer: For all $x < t$, $[t' ≤ x$ and $t' < t] = [t' ≤ x]$)
</span>

$= F(x)/F(t)$.

So, the conditional cdf is $F(x)/F(t)$. What's the conditional density?
<span class="yellow-box">
Answer: $f(x)/F(t)$.
</span>

<span class="dark-mustard-text">**Finding $B$**</span>

Thus $t^2 = e(t) = F(t)E[B(x) | x < t]$
$= F(t)\int_0^t B(x)d[F(x)/F(t)]$
$= \int_0^t B(x)dF(x) = \int_0^t B(x)dx$

Differentiating gives $B(t) = 2t$.

<span class="dark-mustard-text">**Sufficiency**</span>

Check that both bidders using $B(t) = 2t$ is a BNE in the 2nd price auction. 

We have shown this is necessary (if both bidders use the same strictly increasing bid function). 

Now we show it's sufficient.

- Suppose the rival, of type $t′$ uses $B$ and so bids $2t′$ 
- The rival's bid ~ $U[0,2]$
- So, bids $b > 2$ give the same payoff as $b = 2$ and can be safely ignored when optimizing.

If a bidder $i$ of type $t$ bids $b$, expected payoff, 
$\pi(t,b) = Prob[i wins]\{t + E[t′|i wins] – E[B(t′)|i wins]\}$.

But, $Prob[i wins] = Prob[B(t′) < b] = Prob[2t′ < b]$
$= Prob[t′ < b/2] = F(b/2) = b/2$ 
$\pi(t,b) = (b/2)\{t + E[t′ | t′ < b/2] – E[2t′ | t′ < b/2]\}$
$= (b/2)(t + b/4 – 2b/4) = (b/2)(t – b/4)$.
Quadratic in $b$, with roots 0 and $4t$. 
Maximized at $b = 2t$.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">**The Winner's Curse**</span>

$E[t′] = \frac{1}{2}$ is the unconditional expectation of $t′$.

But, conditional on winning with a bid of $b \in [0,2]$, the expectation of $t′$ is $E[t′ | t′ < b/2] = b/4$.

<span class="red-box">
In a common-value auction, learning that one has won the auction provides bad news about the value of the prize. 

This effect is called the <b>winner's curse</b>.
</span>

Some people used to think that this led oil executives to overbid on oil tracts and lose money on average. 

Now, we tend to think that bidders learn to take the effect into account and bid more conservatively because of it.

<span class="yellow-box">
There are many other BNE in this 2nd price common-value auction example. 

Exercise: Find as many as you can.
</span>

The `<span>` tags with the `display: block;` style should work similarly to the `<div>` tags for creating the horizontal lines. Let me know if this resolves the issue!