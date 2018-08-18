# Machine Learning Interview

## Questions:ALgorithsm/Theory
### Q1- What's the trade-off between bias and variance?
  - Bias is error dua to erroneous or overly simplistic assumptions in ther learning algorithms you're using. This can lead to the model underfitting your data, making it hard for it to have high predictive accurary and for you to generalize your knowledge from the training set to the test set.
  - Variance is error due to too much complexity in the learning algorithm you're using. THis leads to the algorithm being highly sensitive to high degrees of variantion in your training data, which can lead your model to overgit the data. You'll be carrying too much too much noise from your training data for your model to be very useful for your test data.
  - The bias-variance decomposition essentially decomposes the learning error from any algorithm by adding the bias, the variance and a bit of irreducible error due to noise in the underlying dataset. Essentially, if you make model more complex and add more variables, you'll lose bias but gain some variance - in order to get the optimally reduced amount of error, you'll have to tradeoff bias and variance. You don't want either high bias or high variance in your model.
  
### Q2- What is the difference between supervised and unsupervised machine learning?
Supervised learning requires training labeled data. For example, in order to do classification (a supervised learning task), you’ll need to first label the data you’ll use to train the model to classify data into your labeled groups. Unsupervised learning, in contrast, does not require labeling data explicitly.
### Q3- How is KNN different from k-means clustering?
k-Nearest Neighbors is a supervised classification algorithms, while k-means clustering is an unsupervised clustering algorithm. while the meachanisms may seem similar at first, what this really means is that in order for K-Nearest Neighbors to work, you need labeled data you want to classify an unlabeled point into( this the nearest neighbor part). K-means clustering requires only a set of unlabeled points and gradually learn how to cluster them into groups by computing the mean of the distance between different points.</br>
The critial difference here is that KNN needs labeled points and is thus supervised learning, while k-means doesn't - and is thus unsupervised learning.
### Q4- Explain how a ROC curve works.
### Q41- How would you simulate the approach AlphaGo took to beat Lee Sidol at Go?
AlphaGo beating Lee Sidol, the best human player at Go, in a best-of-five series was a truly seminal event in the history of machine learning and deep learning. THe Nature paper above describes how this was accomplished with "Monte-Carlo tree search with deep neural networks that been trained by suppervised learning, from human expert games, and by reinforcement learning from games of self-play"
