# variance-reduction

Standard Monte Carlo integration approximates an expected value ***E[g(X)]*** when the function ***g(X)*** and distribution of ***X*** are known, but the expected value can't be computed analytically. Instead, we draw independent ***x_i*** from the distribution of ***X***, compute ***g(x_i)***, and then use the sample mean of ***g(x_i)*** as the approximation for ***E[g(X)]***. However, standard Monte Carlo often samples points ***x*** where ***g(x)*** is zero, resulting in a higher approximation error variance. 

Through importance sampling, we can reduce the variance of the approximation error in standard Monte Carlo by sampling the points ***x_i*** where ***g(x_i)*** is large and then normalize this with the true probability of sampling such points. We do this by choosing a distribution for a new random variable ***Y***. The specific distribution of ***Y*** depends on where ***g(x)*** is largest.


## Resources
* [The Monte Carlo Method](https://statlect.com/asymptotic-theory/Monte-Carlo-method)
* [Importance Sampling](https://www.statlect.com/asymptotic-theory/importance-sampling)

