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
### Q22- How do you ensure you're not overfitting with a model?
This is a simple restatement of a fundamental problem in machine learning: the possibility of overfitting training data and carrying the noise of that data through to the test set, thereby provideing inaccurate generalization.
There are three main methods to avoid overfitting:

### Q23- What ecaluation approaches would you work to gauge the effectiveness of a mchine learning model?
You would first split the dataset into training and test sets, or perhaps use cross-validation 
### Q24- How would you evaluate a logistic regression model?
A subsection of the question above. You have to demonstrate an understanding of what the typical goals of a logistic regression are(classification, prediction etc) and bring up a few examples and use cases.
### Q25- What's the "kernel trick" and how is it useful?
The Kernel trick involves kernel functions that can enable in higher-dimension spaces without explicity calculating the coordinates of points within that dimension: instead, kernel functions compute the inner products between the images of all pairs of data in a feature space. This allows them the very useful attribute of calculating the coordinates of higher dimensions while being computationally cheaper than the explicit calculation of said coordinates. Many algorithms can be expressed in terms of inner products. Using the kernel trick enables us effectively run algorithms in a high-dimensional space with lower-dimensional data.
### Q37- What are your favorite use cases of machine learning models?
### Q38- How would you approach the “Netflix Prize” competition?
The Netflix Prize was a famed competition where Netflix offered $1,000,000 for a better collaborative filtering algorithm. The team that won called BellKor had a 10% improvement and used an ensemble of different methods to win. Some familiarity with the case and its solution will help demonstrate you’ve paid attention to machine learning for a while.
### Q39- Where do you usually source datasets?
Machine learning interview questions like these try to get at the heart of your machine learning interest. Sombody who is truly passionate about machine learning will have gone off and done side projects on their own, and have a good idea of what great datasets are out there. If you're missing any, check out **Quandl** for economic and financial data, and Kaggle's Datasets collection for another great list.
###  Q40- How do you think Google is training data for self-driving cars?
Machine learning interview questions like this one really test your knowledge of different machine learning methods, and your inventiveness if you don't know the answer. Google is currently using recaptcha to source labelled data on storefronts and traffice signs. They are also building on training data collected by Sebastian Thrun at GoogleX - some of which was obtained by his grad students driving buggies on desert dunes!
### Q41- How would you simulate the approach AlphaGo took to beat Lee Sidol at Go?
AlphaGo beating Lee Sidol, the best human player at Go, in a best-of-five series was a truly seminal event in the history of machine learning and deep learning. THe Nature paper above describes how this was accomplished with "Monte-Carlo tree search with deep neural networks that been trained by suppervised learning, from human expert games, and by reinforcement learning from games of self-play"
