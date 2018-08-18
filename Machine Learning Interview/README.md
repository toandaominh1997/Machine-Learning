# Machine Learning Interview

## Questions:ALgorithsm/Theory
### Q1- What's the trade-off between bias and variance?
  - Bias is error dua to erroneous or overly simplistic assumptions in ther learning algorithms you're using. This can lead to the model underfitting your data, making it hard for it to have high predictive accurary and for you to generalize your knowledge from the training set to the test set.
  - Variance is error due to too much complexity in the learning algorithm you're using. THis leads to the algorithm being highly sensitive to high degrees of variantion in your training data, which can lead your model to overgit the data. You'll be carrying too much too much noise from your training data for your model to be very useful for your test data.
  - The bias-variance decomposition essentially decomposes the learning error from any algorithm by adding the bias, the variance and a bit of irreducible error due to noise in the underlying dataset. Essentially, if you make model more complex and add more variables, you'll lose bias but gain some variance - in order to get the optimally reduced amount of error, you'll have to tradeoff bias and variance. You don't want either high bias or high variance in your model.
  
