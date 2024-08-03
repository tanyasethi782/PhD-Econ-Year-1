Sure! Here is the transcription formatted for Obsidian with LaTeX math notation:


## First Borel-Cantelli Lemma

The first Borel-Cantelli Lemma gives a sufficient condition for an event to occur only finitely often.

**Statement**:
Let $\{A_n\}$ be a sequence of events in a probability space. If the sum of the probabilities of these events is finite, then the probability that infinitely many of these events occur is zero. Formally, if
\[ \sum_{n=1}^{\infty} P(A_n) < \infty, \]
then
\[ P\left(\limsup_{n \to \infty} A_n \right) = 0. \]

Here, $\limsup_{n \to \infty} A_n$ denotes the event that infinitely many of the $A_n$ occur, i.e.,
\[ \limsup_{n \to \infty} A_n = \bigcap_{k=1}^{\infty} \bigcup_{n=k}^{\infty} A_n. \]

### Interpretation
If the total probability of the events $A_n$ is finite, then with probability 1, only a finite number of these events will happen.

### Example
Suppose $A_n$ represents the event that the $n$-th digit of a randomly chosen number from $[0, 1]$ is 7. Each $A_n$ has probability $P(A_n) = \frac{1}{10}$. The sum of these probabilities is
\[ \sum_{n=1}^{\infty} P(A_n) = \sum_{n=1}^{\infty} \frac{1}{10} = \infty. \]
According to the first Borel-Cantelli Lemma, we cannot conclude that infinitely many $A_n$ occur. Instead, we need to consider the second lemma for more insight.

## Second Borel-Cantelli Lemma

The second Borel-Cantelli Lemma provides a necessary and sufficient condition for an event to occur infinitely often, under the assumption of independence.

**Statement**:
Let $\{A_n\}$ be a sequence of independent events. If the sum of the probabilities of these events is infinite, then the probability that infinitely many of these events occur is one. Formally, if
\[ \sum_{n=1}^{\infty} P(A_n) = \infty, \]
and the events $A_n$ are independent, then
\[ P\left(\limsup_{n \to \infty} A_n \right) = 1. \]

### Interpretation
If the events $A_n$ are independent and their total probability is infinite, then with probability 1, infinitely many of these events will happen.

### Example
Suppose $A_n$ represents the event that a fair coin lands heads on the $n$-th toss. Each $A_n$ has probability $P(A_n) = \frac{1}{2}$. The sum of these probabilities is
\[ \sum_{n=1}^{\infty} P(A_n) = \sum_{n=1}^{\infty} \frac{1}{2} = \infty. \]
The events are independent (each coin toss does not affect the others). By the second Borel-Cantelli Lemma, the probability that heads appears infinitely often is 1.

## Summary
- **First Borel-Cantelli Lemma**: If the sum of the probabilities of a sequence of events is finite, the probability that infinitely many of them occur is zero.
- **Second Borel-Cantelli Lemma**: If the events are independent and the sum of their probabilities is infinite, the probability that infinitely many of them occur is one.

These lemmas help in understanding the long-term behavior of sequences of random events in probability theory.
