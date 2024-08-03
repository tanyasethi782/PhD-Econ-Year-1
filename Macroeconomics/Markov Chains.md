* **Markov Property** 
A stochastic process has the Markov property if the [conditional probability distribution](https://en.wikipedia.org/wiki/Conditional_probability_distribution "Conditional probability distribution") of future states of the process (conditional on both past and present values) depends only upon the present state; that is, given the present, the future does not depend on the past.

* Markov Chains 
![[Pasted image 20240131111809.png]]
==A discrete-time random process involves a system which is in a certain state at each step, with the state changing randomly between steps==
The Markov property states that the [conditional probability distribution](https://en.wikipedia.org/wiki/Conditional_probability_distribution "Conditional probability distribution") for the system at the next step (and in fact at all future steps) depends only on the current state of the system, and not additionally on the state of the system at previous steps.

Since the system changes randomly, it is generally impossible to predict with certainty the state of a Markov chain at a given point in the future. However, the statistical properties of the system's future can be predicted

**
* **State Spaces**
State spaces are useful in [computer science](https://en.wikipedia.org/wiki/Computer_science "Computer science") as a simple model of machines. Formally, a state space can be defined as a [tuple](https://en.wikipedia.org/wiki/Tuple "Tuple") [_N_, _A_, _S_, _G_] where:

- _N_ is a [set](https://en.wikipedia.org/wiki/Set_(mathematics) "Set (mathematics)") of states
- _A_ is a set of arcs connecting the states
- _S_ is a nonempty [subset](https://en.wikipedia.org/wiki/Subset "Subset") of _N_ that contains start states
- _G_ is a nonempty subset of _N_ that contains the goal states.