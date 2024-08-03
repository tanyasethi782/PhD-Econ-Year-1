## Intro (wiki)
In [probability theory](https://en.wikipedia.org/wiki/Probability_theory "Probability theory") and [statistics](https://en.wikipedia.org/wiki/Statistics "Statistics"), the **characteristic function** of any [real-valued](https://en.wikipedia.org/wiki/Real-valued "Real-valued") [random variable](https://en.wikipedia.org/wiki/Random_variable "Random variable") completely defines its [probability distribution](https://en.wikipedia.org/wiki/Probability_distribution "Probability distribution"). If a random variable admits a [probability density function](https://en.wikipedia.org/wiki/Probability_density_function "Probability density function"), then the characteristic function is the [Fourier transform](https://en.wikipedia.org/wiki/Fourier_transform "Fourier transform") of the probability density function. Thus it provides an alternative route to analytical results compared with working directly with [probability density functions](https://en.wikipedia.org/wiki/Probability_density_function "Probability density function") or [cumulative distribution functions](https://en.wikipedia.org/wiki/Cumulative_distribution_function "Cumulative distribution function"). There are particularly simple results for the characteristic functions of distributions defined by the weighted sums of random variables.

In addition to [univariate distributions](https://en.wikipedia.org/wiki/Univariate_distribution "Univariate distribution"), characteristic functions can be defined for vector- or matrix-valued random variables, and can also be extended to more generic cases.

The characteristic function always exists when treated as a function of a real-valued argument, unlike the [moment-generating function](https://en.wikipedia.org/wiki/Moment-generating_function "Moment-generating function"). There are relations between the behavior of the characteristic function of a distribution and properties of the distribution, such as the existence of moments and the existence of a density function.

The characteristic function is a way to describe a [random variable](https://en.wikipedia.org/wiki/Random_variable "Random variable"). The **characteristic function**,
![[Pasted image 20231027153138.png]]
a function of _t_, completely determines the behavior and properties of the probability distribution of the random variable _X_. The characteristic function is similar to the [cumulative distribution function](https://en.wikipedia.org/wiki/Cumulative_distribution_function "Cumulative distribution function"),

![[Pasted image 20231027153152.png]]

(where **1**{_X ≤ x_} is the [indicator function](https://en.wikipedia.org/wiki/Indicator_function "Indicator function") — it is equal to 1 when _X ≤ x_, and zero otherwise), which also completely determines the behavior and properties of the probability distribution of the random variable _X_. The two approaches are equivalent in the sense that knowing one of the functions it is always possible to find the other, yet they provide different insights for understanding the features of the random variable. Moreover, in particular cases, there can be differences in whether these functions can be represented as expressions involving simple standard functions.

If a random variable admits a [density function](https://en.wikipedia.org/wiki/Probability_density_function "Probability density function"), then the characteristic function is its [Fourier dual](https://en.wikipedia.org/wiki/Duality_(mathematics) "Duality (mathematics)"), in the sense that each of them is a [Fourier transform](https://en.wikipedia.org/wiki/Fourier_transform "Fourier transform") of the other. If a random variable has a [moment-generating function](https://en.wikipedia.org/wiki/Moment-generating_function "Moment-generating function") ��(�)![M_{X}(t)](https://wikimedia.org/api/rest_v1/media/math/render/svg/34fcd0a5942fd5fd42e0f8a7d15c301f9851fbe2), then the domain of the characteristic function can be extended to the complex plane, and

![[Pasted image 20231027153210.png]]

Note however that the characteristic function of a distribution always exists, even when the [probability density function](https://en.wikipedia.org/wiki/Probability_density_function "Probability density function") or [moment-generating function](https://en.wikipedia.org/wiki/Moment-generating_function "Moment-generating function") do not.

The characteristic function approach is particularly useful in analysis of linear combinations of independent random variables: a classical proof of the [Central Limit Theorem](https://en.wikipedia.org/wiki/Central_Limit_Theorem "Central Limit Theorem") uses characteristic functions and [Lévy's continuity theorem](https://en.wikipedia.org/wiki/L%C3%A9vy%27s_continuity_theorem "Lévy's continuity theorem"). Another important application is to the theory of the [decomposability](https://en.wikipedia.org/wiki/Indecomposable_distribution "Indecomposable distribution") of random variables.


## Fourier Transformation 

In [physics](https://en.wikipedia.org/wiki/Physics "Physics") and [mathematics](https://en.wikipedia.org/wiki/Mathematics "Mathematics"), the **Fourier transform** (**FT**) is a [transform](https://en.wikipedia.org/wiki/Integral_transform "Integral transform") that converts a [function](https://en.wikipedia.org/wiki/Function_(mathematics) "Function (mathematics)") into a form that describes the frequencies present in the original function. The output of the transform is a [complex](https://en.wikipedia.org/wiki/Complex_number "Complex number")-valued function of frequency. The term _Fourier transform_ refers to both this complex-valued function and the [mathematical operation](https://en.wikipedia.org/wiki/Operation_(mathematics) "Operation (mathematics)"). When a distinction needs to be made the Fourier transform is sometimes called the [frequency domain](https://en.wikipedia.org/wiki/Frequency_domain "Frequency domain") representation of the original function. The Fourier transform is analogous to decomposing the [sound](https://en.wikipedia.org/wiki/Sound "Sound") of a musical [chord](https://en.wikipedia.org/wiki/Chord_(music) "Chord (music)") into terms of the [intensity](https://en.wikipedia.org/wiki/Sound_intensity "Sound intensity") of its constituent [pitches](https://en.wikipedia.org/wiki/Pitch_(music) "Pitch (music)").

## Questions 
* Problem Set 5 makes use of the characteristic function 
	* [[TS_MetricsPS5.pdf]]
	* Problem 3 could also be done by using the independence formula for characteristic function (not completely sure but there is a formula to check independence)
	