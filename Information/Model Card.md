## MODEL CARD

**Overview**: The modeling approach follows a standard Bayesian Optimization framework using a Gaussian process as the core surrogate model.

**Intended use**: The method is designed to guide query selection when searching for the optimum of an unknown function. It is not intended for applications outside this optimization setting.

**Details**: My modeling strategy has been largely stable over time; it has changed very little from week to week. In the earliest stages, I made small improvements by incorporating limited prior knowledge about specific functions, but otherwise the approach has remained stable. The main differences occur across functions. Functions 1 and 2 have only two features, which makes it possible to visualize them directly. These visualizations significantly aided my decisions when selecting weekly queries.

**Performance**: Assessing query quality is inherently difficult because the true optimum is unknown. However, if one uses instances where the observed best value improves as the metric, then I have observed progress almost every week. This suggests that the queries have been effective.

**Assumptions and limitations**: The approach relies heavily on the assumption that the underlying functions are sufficiently regular, which is essential for Bayesian Optimization to perform well. When using a Gaussian process, it also assumes properties such as constant noise variance across the feature space, which may not hold for all functions. Naturally, the method should be used cautiously outside settings where these assumptions are reasonable, as its optimality is defensible only within those conditions.

**Ethical considerations**: Applying this method in real-world contexts requires caution, as it was developed for a simulated and controlled environment. The results should be reproducible for anyone with access to the Capstone portal.
