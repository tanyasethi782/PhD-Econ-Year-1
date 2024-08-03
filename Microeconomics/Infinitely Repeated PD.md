# Grim Trigger Strategy 
* In finitely repeated game the SPE had each player chooses D at each info set
* When can players choose C at each point along the Equilbrium path: 
	* When discount factor is close to 1 i.e. people care a lot about the future 
	* Choosing C is not SPPE. Not even Nash. 
	* How can you achieve this then?  By using ==Grim Trigger Strategy:== You play C until the other plays D and then you play D forever. It does not say what you do when you choose D. But if you choose D once, you have to choose D forever because the other player will always choose D.  
		* If they stick to the strategy: Players will always choose C. 
	* Is GTS a SPE? : Yes. How to find it?: Look at the change in discounted value after m periods of cooperation and then defection with forever cooperation. 
	* $\delta = \frac{1}{1+r}$ implies that $\delta$ comes from the financial rate of return. 

# Folk Theorem 
* Concepts: 
	* Average Per-Period Payoff:  
	* Minmax (Minimax) Payoffs: Worst case scenario but you are still behaving rationally/ still pursuing your best-response
		$min$ $max$ $u_i(s_i, s_-i)$  // Does the order of min max matter? 
	* (Strictly) Individually Rational Set: 
	 ![[Pasted image 20240328113943.png]]
	* Feasible Payoffs: 
	* FEasible Region 
		* Allows randomization. The strategies are coordinated, With some probability play (1,1), with some probability play something else 

*How do we have the region from the points?:* The payoffs are on the axis so it is just stating what are the possible payoffs, if we are playing with a probability.  


	![[Pasted image 20240328114309.png]]

* Folk Theorem applied to PD:  The folk theorem applied to the Infinitely Repeated prisoners' dilemma says: any APP pair that is both feasible and <u>strictly individually rational</u> can be supported as a SPE if $\delta$ is close enough to 1
	![[Pasted image 20240328114953.png]]

	* Intuition: 