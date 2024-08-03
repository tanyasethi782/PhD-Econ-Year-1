
# Starting Definitions 


## Nash Equilibrium 
Nash Equilibrium: Each player's strategy is best response to the other player 
* Prove Mixed Strategy with p=1/2, 1/2 is unique NE in matching pennies game. 
## Strategy
The **strategy** concept is sometimes (wrongly) confused with that of a **move**. A **move** is an action taken by a player at some point during the play of a game (e.g., in chess, moving white's Bishop a2 to b3). ==A **strategy** on the other hand is a complete [algorithm](https://en.wikipedia.org/wiki/Algorithm "Algorithm") for playing the game, telling a player what to do for every possible situation throughout the game==. It is helpful to think about a "strategy" as a list of directions, and a "move" as a single turn on the list of directions itself. This strategy is based on the payoff or outcome of each action. The goal of each agent is to consider their payoff based on a competitors action. For example, competitor A can assume competitor B enters the market. From there, Competitor A compares the payoffs they receive by entering and not entering. The next step is to assume Competitor B does not enter and then consider which payoff is better based on if Competitor A chooses to enter or not enter. This technique can identify dominant strategies where a player can identify an action that they can take no matter what the competitor does to try to maximize the payoff. This also helps players to identify Nash equilibrium which are discussed in more detail below.

## Strategy Profile 
A **strategy profile** (sometimes called a **strategy combination**) is a set of strategies for all players which fully specifies all actions in a game. ==A strategy profile must include one and only one strategy for every player==

## Finite Vs infinite Strategy Set 
A player's **strategy set** defines what strategies are available for them to play. A strategy profile is a list of strategy sets, ordered from most to least desirable.

==A player has a **finite** strategy set if they have a number of discrete strategies available to them.== 
* For instance, a game of [rock paper scissors](https://en.wikipedia.org/wiki/Rock_paper_scissors "Rock paper scissors") comprises a single move by each player—and each player's move is made without knowledge of the other's, not as a response—so each player has the finite strategy set {rock paper scissors}.

A strategy set is infinite otherwise. 
* For instance the [cake cutting game](https://en.wikipedia.org/wiki/Fair_division "Fair division") has a bounded continuum of strategies in the strategy set {Cut anywhere between zero percent and 100 percent of the cake}.

## Pure Vs Mixed Strategy 
A **pure strategy** provides a complete definition of how a player will play a game. 
* Pure strategy can be thought about as a singular concrete plan subject to the observations they make during the course of the game of play.
* ==In particular, it determines the move a player will make for any situation they could face.== 
* A player's **strategy set** is the set of pure strategies available to that player.

A **mixed strategy** is an assignment of a [probability](https://en.wikipedia.org/wiki/Probability "Probability") to each pure strategy.
* ==When enlisting mixed strategy, it is often because the game does not allow for a rational description in specifying a pure strategy for the game.== This allows for a player to randomly select a pure strategy. (See the following section for an illustration.) 
* ==Since probabilities are continuous, there are infinitely many mixed strategies available to a player.== 
* Since probabilities are being assigned to strategies for a specific player when discussing the payoffs of certain scenarios the payoff must be referred to as "expected payoff".

------
---
# Nash's Theorem 

==Nash showed that there is a Nash equilibrium, possibly in  mixed strategies for every finite game==

Proof: 
Theorems
