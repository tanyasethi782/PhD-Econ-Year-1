Here is the transcription of the file you provided, formatted as requested:

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Optimal Auctions*</span>
(Optimal for the seller, that is.)

==It turns out that (in the symmetric case considered) the auctions with the optimal threshold/reserve price we just found are the best way of selling for the seller.== 

How do we prove this?

We consider the class of all mechanisms the seller could choose. 

==A mechanism is just a game in which the players send messages and the outcome, i.e. allocation of the object and the payments, are determined by the messages sent.==

In an auction, the messages are the bids. 

Other mechanisms could involve offers and counteroffers.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Mechanisms</span>

We are assuming that bidders are risk-neutral.

Then, the expected payoff to i is $p_i t_i – e_i$, where

$p_i$ is i's probability of winning,
$t_i$ is i's type/value, and $e_i$ is i's expected payment.

Since mechanisms are games of incomplete information, the concept of BNE applies.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Revelation Principle</span>

Instead of the seller optimizing over the set of all mechanisms, which may include very complicated ones, it is sufficient for the seller to consider only a subset of these, by the revelation principle.

The revelation principle says that a BNE of any mechanism, no matter how complicated, may be replaced by an equivalent one that is relatively simple, called an incentive compatible, direct mechanism.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Revelation Principle</span>

The Revelation Principle says:

=="Any BNE of a mechanism can be replaced by an equivalent incentive-compatible direct mechanism."==

Direct: i's message space is the set of i's possible types $T_i$, so a strategy for player i is to announce some $s ∈ T_i$

Direct mechanisms are also sometimes called revelation mechanisms, (because players can reveal their types).

Incentive-compatible: it is a BNE for each type of each player to announce her true type.

Equivalent: same allocation and payments.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Optimal Mechanism for the seller</span>

We will find an optimal, voluntary, incentive-compatible direct mechanism for the seller. 

("Voluntary" means that the seller can't force the bidders to participate.)

It then follows, from the revelation principle, that we have found an optimal voluntary mechanism for the seller (without any further qualification).

Reason: ==There couldn't be a non-direct one that's better than all the direct ones, because, for each non-direct one, there's an equivalent direct one.==

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Revelation Principle: Intuition</span>

How can the mechanism designer replace a BNE of an arbitrary mechanism G by an equivalent incentive-compatible direct mechanism?

The designer provides the players with an equivalent, "lazy" version of G.

Instead of choosing (possibly complicated) messages, each player i just announces a type $s_i$.

For each player i, the designer first finds the message that type $s_i$, would choose in the BNE of G. ==The designer then figures what the outcome of G would be if these were the messages sent, and then allocates the prize and determines payments accordingly.==

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Revelation Principle: Intuition</span>

If all other players are announcing their true types, then the strategies chosen for the others are just the same as in the BNE of G. 

Therefore, announcing your true type (which induces your type's BNE strategy) is optimal.  

If not, your type could not have been responding optimally in the BNE of G.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">More Formally…</span>

A bit more formally, how can one replace a BNE of an arbitrary mechanism G by an equivalent incentive-compatible direct mechanism?

Recall that G is a game of incomplete information with the set of players I = {1, …, n}, and player $i ∈ I$ having type $t_i ∈ T_i$

Suppose the BNE strategy profile of G is $a^*_i(t_i)$ for $i ∈ I$ & $t_i ∈ T_i$

Consider the following direct mechanism:
If each $i ∈ I$ announces $s_i ∈ T_i$, 
then the game G is played according to the strategy profile 
$(a^*_1(s_1), a^*_2(s_2), …, a^*_n(s_n))$;
allocation and payments are exactly as if this is the strategy profile chosen in the original game G.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">More Formally…</span>

Then, in this direct mechanism, announcing true types is a BNE because, in G, $a^*_i(t_i)$ is a best response to $a^*_j(t_j)$ $∀j≠i$

We first illustrate this for a specific example and then (again) discuss why it is true in general. The example also introduces some key concepts and notation.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Example: IPV 1st –price Auction</span>

Example: IPV 1st-price auction with 2 risk-neutral bidders with types $t_i$ ~ iid U[0, 1].

Recall the symmetric BNE $B(t_i) = t_i/2$

Replace this by a direct mechanism. If 1 announces $s_1 ∈ [0, 1]$ and 2 announces $s_2 ∈ [0, 1]$, this translates to bids $s_1/2$ and $s_2/2$

So, i wins the object and pays $s_i/2$ if $s_i$ exceeds $s_j$ (with each getting the object and paying $s_i/2$ with probability ½ in case of a tie).

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Introducing $\underline{p_i}(s_i, s_{-i})$ and $\bar{e_i}(s_i, s_{-i})$</span>

Bidder i's expected payoff is 
(Probability of winning)$t_i$ – expected payment.

We can express both the probability of winning and the expected payment as functions of everyone's announcement..
Here the other player* is denoted by the subscript –i.

Probability of winning $p_i(s_i, s_{-i}) = 1$ if $s_i > s_{-i}$
			   $= ½$ if $s_i = s_{-i}$
			   $= 0$ if $s_i < s_{-i}$.

Expected Payment $e_i(s_i, s_{-i}) = s_i p_i(s_i, s_{-i})/2$. 

\* More generally, with more than two bidders/participants, $s_{-i}$ indexes the vector of announcements of all participants other than i.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Introducing $p_i(s_i)$ and $e_i(s_i)$
(now assuming the rival announces her true type)</span>

If i's rival announces her true type, then $s_{-i} = t_{-i}$ ~ U[0,1].

Let $E_{-i}$ denote i's expectation with respect to $t_{-i}$.

The expected values of $p_i$ and $e_i$ with respect to $t_{-i}$ are functions of i's choice $s_i$ only:

$p_i(s_i) = E_{-i}[p_i(s_i, t_{-i})]$
$= Prob[t_{-i} < s_i] = F(s_i) = s_i$;

$e_i(s_i) = E_{-i}[e_i(s_i, t_{-i})]$  
$= s_i^2/2$.

Bidder i's expected payoff $π_i(s_i,t_i)$ is a function of her announcement $s_i$ and her true type $t_i$: 

$π_i(s_i,t_i) = p_i(s_i)t_i − e_i(s_i) = s_i t_i − s_i^2/2$

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Example</span>

$π_i(s_i, t_i) = s_i t_i − s_i^2/2$ 
$= (s_i/2)(2t_i − s_i)$.

Quadratic in $s_i$ with roots 0 and $2t_i$.

Maximized at $s_i = t_i$.

So, it's best for i to announce her true type.

In other words, for this mechanism, if your rival announces her true type, then it is optimal for you to do so as well: i.e., the mechanism is incentive-compatible.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Why truth telling is a BNE</span>

More generally, if $(a^*_1(t_1), a^*_2(t_2), …, a^*_n(t_n))$ is a BNE of the original mechanism, then, for each* type $t_i$ of each player i, $a^*_i(t_i)$ maximizes $E_{-i}[u_i(a_i, a^*_{-i}(t_{-i}))]$ w.r.t. $a_i$.

Thus $t_i$ maximizes $E_{-i}[u_i(a^*_i(s_i), a^*_{-i}(t_{-i}))]$ w.r.t. $s_i$.

In words:  
In the BNE of the original mechanism, the BNE choice for your true type was optimal given everyone else's BNE choice. In the direct mechanism, each player will be given the BNE choice of whatever type she announces. Thus, it's optimal in the direct mechanism to announce your true type, if everyone else is announcing their true type.

\*Really should be for "almost" each type $t_i$ of each player i---we don't care what happens on sets with probability zero.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Optimal Auctions: Assumptions</span>

Recall, the seller is risk-neutral, values the object at $t_0 ≥ 0$

n risk-neutral bidders i = 1, 2,…, n. 

Independent Private Values $t_i$ ~ $F_i$.
Independent but needn't have same distribution.

$F_i$ has support $T_i = [a_i, b_i]$ ⊂ ℝ+ and density $f_i > 0$ on $(a_i, b_i)$.

∀i, define $M_i(t_i) = t_i − [1 − F_i(t_i)]/f_i(t_i)$. 
(Recall that $M_i(t_i)$ would be the expected marginal revenue if i were the sole bidder and the price were set at $t_i$).

Assume that $M_i(t_i)$ is increasing in $t_i$ on $T_i$.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Some Notation</span>

$T = T_1 \times T_2 \times ... \times T_n$;
$t ∈ T$, $t = (t_1, t_2, …, t_n) = (t_i, t_{-i})$; 
$s ∈ T$, $s = (s_1, s_2, …, s_n) = (s_i, s_{-i})$.

A direct mechanism maps each announced-types vector $s ∈ T$ to $p(s)$ and $e(s)$.

$p(s) ∈ ℝ^n_+$, and $p_i(s)$ is the probability that i wins if the vector of announced types is s.

$Σ_i p_i(s) ≤ 1$ and $p_0(s) = 1 − Σ_i p_i(s) ≥ 0$ is the probability that the seller keeps the object/prize.

$e(s) ∈ ℝ^n$, and $e_i(s)$ is the expected payment by i if the vector of announced types is s. 

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Optimal auction</span>

By the revelation principle, we need to consider only incentive-compatible direct mechanisms, i.e. ones for which it is optimal to be truthful if everyone else is.

Fix the mechanism $\mathcal{m} = (p, e)$, and bidder i, and suppose that all others are telling the truth.

If i is of type $t_i$ and announces $s_i$ then i's expected payoff:

$π_i(s_i, t_i) = E_{-i}[p_i(s_i, t_{-i})t_i − e_i(s_i, t_{-i})]$
       $= p_i(s_i)t_i − e_i(s_i)$, where
$p_i(s_i) = E_{-i}[p_i(s_i , t_{-i})]$ and $e_i(s_i) = E_{-i}[e_i(s_i, t_{-i})]$ 

and $E_{-i}$ denotes expectation with respect to $t_{-i}$

Note that $∂π_i(s_i,t_i)/∂t_i = p_i(s_i)$.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Envelope theorem</span>

Also, for each given $s_i$

$π_i(s_i, t_i) = p_i(s_i)t_i − e_i(s_i)$ 
is an affine function of I apologize for the oversight. Here is the full transcription of the provided document, formatted as requested:

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Envelope theorem</span>

Also, for each given $s_i$

$π_i(s_i, t_i) = p_i(s_i)t_i − e_i(s_i)$
is an affine function of $t_i$ (thus convex and concave).

Since the mechanism is incentive-compatible, i's equilibrium expected payoff:
$u_i(t_i) = \max π_i(s_i, t_i)$  $∀s_i ∈ T_i$
         $=π_i(t_i, t_i)$. (1)

By the envelope theorem, wherever $u_i$ is differentiable, 
$u'_i(t_i) = ∂π_i(s_i, t_i)/∂t_i |_{s_i=t_i} = p_i(t_i)$

We can draw some pictures to illustrate.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

For a single given $s_i$

$π_i(s_i, t_i) = p_i(s_i)t_i − e_i(s_i)$

[Image: Graph showing Expected payoff if true type is $t_i$ and announced type is $s_i$ as a function of True type $t_i$ from $a_i$ to $b_i$]

$π_i(s_i, t_i) = p_i(s_i)t_i − e_i(s_i)$

[Image: Graph showing $π_i(s_i, t_i)$ for several $s_i$ as functions of True type $t_i$ from $a_i$ to $b_i$]

$u_i(t_i)$ is the upper envelope of $π_i(s_i, t_i)$ for all $s_i ∈ T_i$

[Image: Graph showing $π_i(s_i, t_i)$ for various $s_i$ and $u_i(t_i)$ as functions of True type $t_i$ from $a_i$ to $b_i$]

If your true type is $t_i = x$, you set $s_i = x$

[Image: Graph showing $u_i(t_i)$ and $π_i(x, t_i) = p_i(x)t_i − e_i(x)$ as functions of True type $t_i$ from $a_i$ to $b_i$ with $x$ marked]

Tangency at point A shows $u'_i(x) = p_i(x)$, illustrating the envelope theorem

[Image: Graph showing Expected Payoff $u_i(t_i)$ and $π_i(x, t_i) = p_i(x)t_i − e_i(x)$ as functions of True type $t_i$ from $a_i$ to $b_i$ with $x$ and tangency point A marked]

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Envelope argument</span>

Because $u_i$ is the maximum of convex functions, $u_i$ is itself convex.

Thus $u_i$ is differentiable except on a set that is at most countable.

Thus $u_i$ is differentiable except on a set of measure zero, and, where the derivative exists, $u'_i(x) = p_i(x)$.

Thus $u_i$ is equal to the integral of its derivative:

$u_i(t_i) = u_i(a_i) + \int_{a_i}^{t_i} p_i(x)dx$

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">The crucial envelope result</span>

$u_i(t_i) = u_i(a_i) + \int_{a_i}^{t_i} p_i(x)dx$

So 
$p_i(t_i)t_i − e_i(t_i) = u_i(t_i)$
           $= u_i(a_i) + \int_{a_i}^{t_i} p_i(x)dx$

$e_i(t_i) = p_i(t_i)t_i − \int_{a_i}^{t_i} p_i(x)dx − u_i(a_i)$

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Seller's problem</span>

The seller chooses a voluntary incentive-compatible direct mechanism to maximize the seller's expected profit:

$\Pi_0 = \int_T \sum_{i=1}^{n} e_i(t) dF(t) + \int_T p_0(t)t_0 dF(t)$

where
$dF(t) = \prod_{i=1}^{n} dF_i(t_i)$

"Voluntary" means bidders are free not to take part, i.e., to opt out. If they opt out, they receive nothing and pay nothing, thus receiving zero payoff.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Participation Constraints</span>

Hence $u_i(t_i) ≥ 0$ $∀i, t_i ∈ T_i$.

These inequalities are called participation constraints. They must be satisfied in order for bidders to be willing to participate in the mechanism.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Seller's Expected Profit</span>

$\Pi_0 = \int_T \sum_{i=1}^{n} e_i(t) dF(t) + \int_T p_0(t)t_0 dF(t)$

where 
$dF(t) = \prod_{i=1}^{n} dF_i(t_i)$

Note that this expression for $dF(t)$ as the product of the $dF_i(t_i)$ terms follows from the independence of the $t_i$.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">A note about notation</span>

Remember that $T_i = [a_i, b_i]$ 
and $T = T_1 \times T_2 \times ... \times T_n$,

So, the integrals above (over the sets $T_i$ and $T$ are just a briefer notation for integrals that can be written out in full as:

$\int_{T_i} e_i(t_i) dF_i(t_i) = \int_{a_i}^{b_i} e_i(t_i) f_i(t_i) dt_i = \int_{a_i}^{b_i} e_i(t_i) dF_i(t_i)$

and

$\int_T p_i(t) dF(t) = \int_{T_1} ... \int_{T_n} p_i(t_1,...,t_n) dF_1(t_1) ... dF_n(t_n) = \int_{a_1}^{b_1} ... \int_{a_n}^{b_n} p_i(t_1,...,t_n) dF_1(t_1) ... dF_n(t_n)$

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

Substituting for the $e_i(t_i)$ expressions gives

<span class="dark-mustard-text">Seller's Expected Profit</span>

$\Pi_0 = \int_T \sum_{i=1}^{n} [p_i(t_i)t_i − \int_{a_i}^{t_i} p_i(x)dx − u_i(a_i)] dF(t) + \int_T p_0(t)t_0 dF(t)$

$= \int_T \sum_{i=1}^{n} p_i(t_i)t_i dF(t) - \sum_{i=1}^{n} \int_{T_i} [\int_{a_i}^{t_i} p_i(x)dx]dF_i(t_i) + \int_T p_0(t)t_0 dF(t)$

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Participation Constraints</span>

Recall that, because the mechanism is voluntary, all bidders are free to opt out, receiving zero payoff so $u_i(t_i) ≥ 0$ $∀i, t_i ∈ T_i$.

Because $u′_i(t_i) = p_i(t_i) ≥ 0$, $u_i$ is nondecreasing in $t_i$, and the above constraints are equivalent to 
$u_i(a_i) ≥ 0$ $∀i$.

Examining the objective on the previous slide shows that these constraints are binding at the optimum.

Thus $u_i(a_i) = 0$ $∀i$.

Can rewrite $e_i(t_i)$ formula…

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Expected payment</span>

$e_i(t_i) = p_i(t_i)t_i − \int_{a_i}^{t_i} p_i(x)dx − u_i(a_i)$
         $= p_i(t_i)t_i − ∫_{a_i}^{t_i} p_i(x)dx$ (1)

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">The $p_i$ functions</span>

Thus, given the $p_i$ functions, for any viable candidate to be the optimal mechanism (i.e. one for which the participation constraints are binding) the $e_i$ are determined by the previous equation. 

Are any $p_i$ functions allowable?

No, incentive compatibility restricts these.

It requires that ∀i $p_i$ be nondecreasing, i.e., if you announce a higher type, your probability of winning does not go down, as we now show.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Incentive Compatibility</span>

Let $π_i(s_i, t_i)$ denote bidder i's expected payoff as a function of announcement $s_i$ and true type $t_i$.

Incentive compatibility can then be expressed: 
∀$t_i$ and $s_i ∈ T_i$,
$π_i(t_i, t_i) ≥ π_i(s_i, t_i)$.

Because this is true for all $t_i$ and $s_i ∈ T_i$,
it's true if 
(i) $x$ is the true type and $y$ the announced type,
and
(ii) if $y$ is the true type and $x$ is the announced type.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Incentive Compatibility</span>

∀$x$ and $y ∈ T_i$ (if $x$ is the true type and $y$ the announced type),

$π_i(x, x) ≥ π_i(y, x)$ 
⇒ $p_i(x)x - e_i(x) ≥ p_i(y)x - e_i(y)$
⇒ $e_i(y) - e_i(x) ≥ [p_i(y) - p_i(x)]x$.

Interchanging $x$ and $y$ (i.e., using $y$ for the true type and $x$ for the announced type) gives
$e_i(x) - e_i(y) ≥ [p_i(x) - p_i(y)]y$

Adding the last two inequalities,
$0 ≥ [p_i(y) - p_i(x)](x - y) = [p_i(y) - p_i(x)](y - x) ≥ 0$

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Incentive Compatibility</span>

The change in $p_i$ (if any) is in the same direction as the change in $x$.

So, for incentive compatibility, (no matter what the $e_i$ functions are) it is necessary that $p_i$ is nondecreasing.

(We will see later that, with the $e_i$ functions given by equation (1) above, it's also sufficient for incentive compatibility that $p_i$ is nondecreasing.)

$\Pi_0 = \int_T \sum_{i=1}^{n} [p_i(t)t_i − \int_{a_i}^{t_i} p_i(x)dx]dF(t) + \int_T p_0(t)t_0 dF(t)$
       $= \int_T \sum_{i=1}^{n} [p_i(t)t_i - [1 - F_i(t_i)]\int_{a_i}^{t_i} p_i(x)dx/[1 - F_i(t_i)]]dF(t) + \int_T p_0(t)t_0 dF(t)$

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

$E_{t_{-i}}[p_i(t_i,t_{-i})] = \int_{T_{-i}} p_i(t) \prod_{j ≠ i} dF_j(t_j)$,
where 
$T_{-i} = \prod_{j ≠ i} T_j$.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Change order of integration</span>

We now do a change in the order of integration

[Image: Graph showing shaded triangle over $x$ from $a_i$ to $t_i$ and $t_i$ from $a_i$ to $b_i$]

[Image: Graph showing two different paths traversing the shaded triangle - one going horizontally first then vertically, the other going vertically first then horizontally]

Of course, my apologies for missing the last part. Here is the transcription of the remainder of the document, formatted as requested:

$\int_{a_i}^{b_i} \int_{a_i}^{t_i} p_i(x)dF_i(x)dt_i = \int_{a_i}^{b_i} p_i(x)[1 - F_i(x)]dx$

$= \int_{a_i}^{b_i} p_i(t_i)[1 - F_i(t_i)]dt_i$
$= \int_{a_i}^{b_i} p_i(t_i) \frac{1 - F_i(t_i)}{f_i(t_i)} f_i(t_i)dt_i$
$= \int_{a_i}^{b_i} p_i(t_i) \frac{1 - F_i(t_i)}{f_i(t_i)} dF_i(t_i)$

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">$M_i(t_i)$</span>

Recall that $t_i - [1 - F_i(t_i)]/f_i(t_i) = M_i(t_i)$ 
is assumed to be increasing in $t_i$

$\Pi_0 = \int_T \sum_{i=1}^{n} [p_i(t)t_i - \int_{a_i}^{t_i} p_i(x)dx]dF(t) + \int_T p_0(t)t_0 dF(t)$
       $= \int_T \sum_{i=1}^{n} [p_i(t)t_i - [1 - F_i(t_i)]\int_{a_i}^{t_i} p_i(x)dx/[1 - F_i(t_i)]]dF(t) + \int_T p_0(t)t_0 dF(t)$
       $= \int_T \sum_{i=1}^{n} [p_i(t)t_i - p_i(t_i) \frac{1 - F_i(t_i)}{f_i(t_i)}]dF(t) + \int_T p_0(t)t_0 dF(t)$
       $= \int_T \sum_{i=1}^{n} p_i(t)M_i(t_i)dF(t) + \int_T p_0(t)t_0 dF(t)$
       $= \int_T \sum_{i=1}^{n} p_i(t)\{M_i(t_i) - t_0\}dF(t) + \int_T t_0 dF(t)$

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Maximum</span>

For each $t$, the sum in curly brackets is a convex combination (i.e. a weighted average) of the $M_i$ and $t_0$

Seller chooses the weights $p_i(t)$ to maximize the sum

This sum is maximized by setting
$p_i(t) = 1$ if $M_i(t_i) > \max \{t_0, \max_{j≠i}M_j(t_j)\}$
         $= 0$ otherwise \*

Ties occur with zero probability because
$t_i$ are independent, continuously distributed, and $M_i$ are strictly increasing

Because $M_i$ are strictly increasing, the above rule \* makes $p_i$ and hence $\bar{p}_i$ nondecreasing in $t_i$ 

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Maximum expected profit</span>

The value of expected profit when this optimal allocation rule is used is just

$Π_0 = E[\max \{t_0, \max_i M_i(t_i)\}]$

sometimes this provides a simple way to compute the maximum expected profit

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Necessary conditions</span>

We have found necessary conditions for a voluntary, incentive-compatible direct mechanism to be optimal for the seller:

For any announced vector $s$ give the object to the bidder $i$ whose value of $M_i(s_i)$ is highest, unless
$M_i(s_i) < t_0$ for all $i$, 
in which case the seller keeps the object.

This determines $p$, and hence $\bar{p}$. 
Ties, which occur with zero probability, can be handled arbitrarily

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Necessary conditions</span>

For each bidder $i$ who announces $s_i$, charge on average the amount:

$e_i(s_i) = p_i(s_i)s_i - \int_{a_i}^{s_i} p_i(x)dx$ 

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Sufficiency</span>

(1) To see that the above characterization is sufficient for optimality, we show that it is
(1) voluntary;
(2) satisfies incentive compatibility; and
(3) makes the objective $Π_0$ at least as high as any other voluntary incentive-compatible mechanism.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">(1) Voluntary</span>

Because $i$ has the option of announcing the lowest type ($a_i$), $i$ gets a payoff of at least zero.

Formally, $∀i, t_i ∈ T_i$
$u_i(t_i) ≥ \max π_i(s_i, t_i)$
         $≥ π_i(a_i, t_i)$
         $= p_i(a_i)t_i − e_i(a_i)$ 
         $= p_i(a_i)t_i − p_i(a_i)a_i$
         $= p_i(a_i)(t_i − a_i) ≥ 0$

So, the mechanism is voluntary.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">(2) Incentive Compatible</span>

To show incentive compatibility, we show that, for any bidder $i$, if $y$ is $i$'s true type the following inequality holds for all $z ∈ T_i$:

[Notation reminder: Recall that we've been using $t$ for the vector of everyone's true type and $s$ for the vector of everyone's announced type. So here, to avoid subscripts, we use $y$ for the true type and $z$ for the announced type.]

$π_i(y,y) ≥ π_i(z,y)$

$(p_i(y)y − e_i(y)) - (p_i(z)y − e_i(z)) ≥ 0$

$p_i(y)y - \int_{a_i}^{y} p_i(x)dx - p_i(z)y + \int_{a_i}^{z} p_i(x)dx$
     $≥ p_i(y)y - p_i(z)y - \int_{z}^{y} p_i(x)dx$
     $=(p_i(y) - p_i(z))(y - z)$

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">(2) Incentive Compatibility</span>

The last condition is true because $p_i$ is nondecreasing 
(Check the cases $z < y$ and $z > y$ separately)

Hint: Draw a graph with a nondecreasing $p$ function and then represent as areas the two sides of the last inequality on the previous slide

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">(3) Optimality</span>

To see that the proposed solution is optimal recall that, for any voluntary, incentive-compatible mechanism, the value of the objective $Π_0$ is bounded above\* by an integral over all $t$ of convex combinations of the $M_i$ and $t_0$ and so is maximized by the rule we specified.

\* it is equal to the bound when the participation constraints are binding

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Optimal among all mechanisms</span>

We have now found an optimal incentive-compatible and voluntary direct mechanism.

[Aside: We say "an" rather than "the" because although the allocation rule $p$ is uniquely determined (except on a set of probability zero), and the expected payment functions $e_i$ are uniquely determined, the payment functions $e_i$ are not uniquely determined.]

But, by the revelation principle, we know that any Bayesian Nash Equilibrium of any mechanism can be replaced by an equivalent incentive-compatible direct mechanism.

Thus, the mechanism we have found is optimal among all voluntary mechanisms (direct or not).

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Symmetric Case</span>

In the symmetric case, ∀i $F_i = F$ and $M_i = M$ and so in an optimal auction the object goes to the bidder of highest type $t_i$ as long as $M(t_i) > t_0$.

This was exactly the allocation in the 1st and 2nd price auction with the optimal reservation price.

In both these auctions the bidder of lowest type $a$ earns payoff 0 and so either of those auctions is the best possible mechanism for the seller.

(Note that they have different $e_i$ functions.)

Exercise: There are many other optimal auctions: for example, find an all-pay auction that is optimal.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Symmetric Case</span>

Even in the symmetric case the optimal auction is typically not efficient, because the seller sets a reserve price that is typically above opportunity cost.

To sell to $i$ to requires that
$M(t_i) = t_i - [1 - F(t_i)]/f(t_i) > t_0$.

This is different from the condition that would apply if there was no private information, and all the $t_i$ were common knowledge: In this case the allocation is efficient, and is to give it to the highest $t_i$ if $t_i > t_0$.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Asymmetric Case</span>

In asymmetric cases, the optimal mechanism discriminates among buyers/bidders

Instead of the object going to the bidder with the highest type, $t_i$, it goes to the bidder with the highest virtual valuation $M_i(t_i)$ as long as $M_i(t_i) > t_0$.

Because $M_i(t_i) = t_i − [1 − F_i(t_i)]/f_i(t_i)$,
we can think of $[1 − F_i(t_i)]/f_i(t_i)$ as representing the extent to which $i$ is being disadvantaged or discriminated against, i.e a "penalty" relative to efficient allocation (i.e. allocation with complete information).

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Asymmetric Case</span>

Recall that $t_i − [1 − F_i(t_i)]/f_i(t_i)$ corresponds to the seller's marginal revenue, and so the "penalty"
$[1 − F_i(t_i)]/f_i(t_i)$ 
corresponds to the part of the buyer's value that does not get added to the seller's revenue, but instead represents the marginal informational rent that goes to the inframarginal buyer types.

Recall that the penalty $[1 − F_i(t_i)]/f_i(t_i)$ is the inverse of the hazard rate at $t_i$ and is related to the inverse of the elasticity of expected demand by bidder $i$ at price $t_i$ which is $[1 − F_i(t_i)]/t_i f_i(t_i)$

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">An Asymmetric Example</span>

Suppose there are 2 bidders in an independent private values model, with $t_1$ ~ U[1,2] and $t_2$ ~ U[0,3], independent. The value to the seller, $t_0$ is 0.

Note that they have the same mean of 1.5, so that both are uniform distributions centered at 1.5 and the only difference is that one is more spread out than the other

Under the usual assumption that the bidders play non-cooperatively, determine how the prize is allocated in an optimal mechanism/auction.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">$t_1$ ~ U[1,2], $t_2$ ~ U[0,3], $t_0 = 0$</span>

$F_i(t_i) = (t_i - a_i)/(b_i - a_i)$, $f_i(t_i) = 1/(b_i - a_i)$,

$M_i(t_i) = t_i - [1 - F_i(t_i)]/f_i(t_i)$
         $= t_i - [1 - (t_i - a_i)/(b_i - a_i)]/[1/(b_i - a_i)]$ 
         $= t_i - (b_i - t_i) = 2t_i - b_i$

$M_1(t_1) = 2t_1 - 2$ and $M_2(t_2) = 2t_2 - 3$

When will 1 get the object (i.e. "win"?)

1 wins if $2t_1 - 2 > 2t_2 - 3$ (and $2t_1 - 2 > 0$, which is almost always true, i.e. true with probability one).

i.e. if $t_1 > t_2 - ½$

2 wins if $t_2 > t_1 + ½$ (and $t_2 > 3/2$, but this is implied by the first inequality for almost all  I apologize, you are correct. Here is the transcription of the remaining part of the document, formatted as requested:

2 wins if $t_2 > t_1 + ½$ (and $t_2 > 3/2$, but this is implied by the first inequality for almost all $t_1$).

The optimal auction here discriminates in favor of bidder 1. 
With a uniform distribution the inverse hazard rate is $b_i - t_i$ and thus bidder 1 tends to have less informational rent to extract.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Key Assumptions used in deriving the Optimal Auction result</span>

Some key assumptions are:
1. Risk neutrality;
2. Monotonicity of the virtual valuation functions $M_i(t_i)$; 
3. Independence;
4. The seller knows the distributions $F_i$.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Relaxing the Assumptions</span>

Risk neutrality: technically hard to relax - need optimal control

Monotonicity of the $M_i(t_i)$
- analogous to MR decreasing or total revenue and profit concave
assumed for convenience 
can drop, but may need deliberate randomness in the mechanism to concavify the problem-- sometimes called ironing).

Independence: If we drop this (but retain the other assumptions) the seller can do much better.
The key idea here is that the seller can now infer the private information for one bidder by offering a fair gamble to another bidder whose type is correlated with the first. Since the seller in equilibrium extracts all private information, the bidders end up with no informational rents, and the seller gets all the available surplus. This full-extraction result depends critically on risk-neutrality.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">Relaxing the Assumptions</span>

The assumption that the seller knows the distributions $F_i$:

Recent work has shown that one can design auctions that simultaneously sell the good and, in effect, use the other bidders' choices to estimate each bidder's type distribution. As the number of bidders of each kind $i$ grows large, expected seller profit converges to the same level as it would be if the distributions were known.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">An optimal mechanism in which truth-telling is weakly dominant</span>

There is a particular, direct-mechanism way to implement the optimal mechanism that is like the 2nd-price auction in that:
(1) only the winner of the object pays; 
(2) announcing one's true type is a weakly dominant strategy (not just a BNE);
(3) the amount the winner pays depends on the most competitive type announced by the other players, not on the winner's announcement.

In fact, the payment by the winner $i$ is just the threshold type for $i$ that marks the line between $i$ winning and $i$ losing, given what the others announce (or, if all announced types of $i$ would win, the payment is just $i$'s lowest possible type, namely $a_i$).

This is described in more detail below.

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

<span class="dark-mustard-text">An advantage of mechanisms in which truth-telling is dominant</span>

If truth-telling is a dominant strategy, then the bidders don't need to know (or make any assumptions about) the other bidders' distribution functions $F_i$

Here's the math describing how the dominant-strategy implementation of the optimal auction works:

Let $y_i(s_{-i}) = \inf\{x_i ∈ T_i: M_i(x_i) ≥ M_j(s_j) ∀j ≠ i, M_i(x_i) ≥ t_0\}$.

Then, in any optimal mechanism, probability of $i$ winning
$p_i(s_i, s_{-i}) = 1$ if $M_i(s_i) > M_j(s_j)$ $∀j ≠ i$ and $M_i(s_i) > t_0$ ⇔ $s_i > y_i(s_{-i})$
                 $= 0$ if $s_i < y_i(s_{-i})$

Consider the payment rule:
$e_i(s_i, s_{-i}) = y_i(s_{-i})$ if $s_i > y_i(s_{-i})$
                 $= 0$ if $s_i < y_i(s_{-i})$

Note that truth-telling ($s_i = t_i$) is weakly dominant.
Reason: it yields a payoff of $t_i - y_i(s_{-i})$ if $t_i > y_i(s_{-i})$, and 0 otherwise.

Changing $s_i$ would just make it possible for $i$ to win the object at a price above her value $t_i$ or lose it when the price is below $t_i$

<span style="display: block; border-bottom: 2px solid #00FFFF; margin: 10px 0;"></span>

Because telling the truth is weakly dominant, the mechanism consisting of the above allocation and payment rule is incentive compatible.

Because the lowest type $a_i$ of each bidder $i$ receives zero expected payoff, this mechanism is voluntary, with the participation constraints binding for $a_i$.

Because, additionally, the allocation of the object is the same as in the optimal mechanism, the mechanism is optimal.

Thus, it has the same $e_i$ functions as characterized earlier for the optimal auction.
