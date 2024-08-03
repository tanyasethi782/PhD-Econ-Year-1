
In [statistics](https://en.wikipedia.org/wiki/Statistics "Statistics"), **maximum likelihood estimation** (**MLE**) is a method of [estimating](https://en.wikipedia.org/wiki/Estimation_theory "Estimation theory") the [parameters](https://en.wikipedia.org/wiki/Statistical_parameter "Statistical parameter") of an assumed [probability distribution](https://en.wikipedia.org/wiki/Probability_distribution "Probability distribution"), given some observed data. This is achieved by [maximizing](https://en.wikipedia.org/wiki/Mathematical_optimization "Mathematical optimization") a [likelihood function](https://en.wikipedia.org/wiki/Likelihood_function "Likelihood function") so that, under the assumed [statistical model](https://en.wikipedia.org/wiki/Statistical_model "Statistical model"), the [observed data](https://en.wikipedia.org/wiki/Realization_(probability) "Realization (probability)") is most probable. 

==The [point](https://en.wikipedia.org/wiki/Point_estimate "Point estimate") in the [parameter space](https://en.wikipedia.org/wiki/Parameter_space "Parameter space") that maximizes the likelihood function is called the maximum likelihood estimate.==




### Relation to minimizing Kullback–Leibler divergence and cross entropy[[edit](https://en.wikipedia.org/w/index.php?title=Maximum_likelihood_estimation&action=edit&section=11 "Edit section: Relation to minimizing Kullback–Leibler divergence and cross entropy")]

Finding �^![{\hat {\theta }}](https://wikimedia.org/api/rest_v1/media/math/render/svg/f0eaae56d74c5844e86caeed8ae205ff9e413bba) that maximizes the likelihood is asymptotically equivalent to finding the �^![{\hat {\theta }}](https://wikimedia.org/api/rest_v1/media/math/render/svg/f0eaae56d74c5844e86caeed8ae205ff9e413bba) that defines a probability distribution (��^![{\displaystyle Q_{\hat {\theta }}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/adc86adb15c404f22a05526777d6b39a12353a76)) that has a minimal distance, in terms of [Kullback–Leibler divergence](https://en.wikipedia.org/wiki/Kullback%E2%80%93Leibler_divergence "Kullback–Leibler divergence"), to the real probability distribution from which our data were generated (i.e., generated by ��0![{\displaystyle P_{\theta _{0}}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/50fe6689cb91e5fb22a2bd8b09719cc87048b6c3)).[[23]](https://en.wikipedia.org/wiki/Maximum_likelihood_estimation#cite_note-23) In an ideal world, P and Q are the same (and the only thing unknown is �![\theta](https://wikimedia.org/api/rest_v1/media/math/render/svg/6e5ab2664b422d53eb0c7df3b87e1360d75ad9af) that defines P), but even if they are not and the model we use is misspecified, still the MLE will give us the "closest" distribution (within the restriction of a model Q that depends on �^![{\hat {\theta }}](https://wikimedia.org/api/rest_v1/media/math/render/svg/f0eaae56d74c5844e86caeed8ae205ff9e413bba)) to the real distribution ��0![{\displaystyle P_{\theta _{0}}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/50fe6689cb91e5fb22a2bd8b09719cc87048b6c3).[[24]](https://en.wikipedia.org/wiki/Maximum_likelihood_estimation#cite_note-24)
