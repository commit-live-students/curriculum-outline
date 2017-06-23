# Week 3: Supervised Machine Learning

* [Day 1] Introduction to Supervised Machine Learning
    - Overview/Review
        * Regression vs Classification
        * Algorithms
        * Metrics
    - Introduction to Linear Algebra (Linear Algebra)
        * Deriving the closed-form solution
        * Examples
            - Univariate
            - Multiple variables
        * Assessing Model
            - Metrics
            - Visualizations
        * Assumptions and their validation
            - Visualizations
    - Introduction to Linear Algebra (Optimization)
        * GD in action
        * Importance of preprocessing (normalization, standardization)
        * Matching results to closed-form solution
        * Closed-form Solution vs Gradient Descent Solution: where and how we use them
    - [Hands-on]
        * Linear Regression on Industry Dataset 1
        * Linear Regression on Industry Dataset 2
        * Writing a report summarizing a Linear Regression model
* [Day 2] Linear and Logistic Regression, Regularization
    - Problems with Linear Regression
        * Linear separability (polynomial features)
        * Assumptions
        * Outliers
    - Logistic Regression
        * Why Logistic Regression?
        * Handling Outliers
        * Assessing model quality (confusion matrix)
    - GD for Logistic Regression
    - Regularization
        * [Why?](http://stats.stackexchange.com/questions/4272/when-to-use-regularization-methods-for-regression?noredirect=1&lq=1)
        * [L1](http://stats.stackexchange.com/questions/200416/is-regression-with-l1-regularization-the-same-as-lasso-and-with-l2-regularizati) + intuition about its effect
        * [L2](http://statweb.stanford.edu/~tibs/sta305files/Rudyregularization.pdf) + intuition about its effect
        * [L1 vs L2](???)
        * [L1 + L2](http://stats.stackexchange.com/questions/184029/what-is-elastic-net-regularization-and-how-does-it-solve-the-drawbacks-of-ridge?rq=1) (short mention)
        * [A worked-out example](https://www.analyticsvidhya.com/blog/2016/01/complete-tutorial-ridge-lasso-regression-python/)
    - Bias-Variance trade-off (revisit for every model)
    - [Hands-on]
        * On industry dataset, build models using
            - Linear Regression
            - Logistic Regression
            - L1 regularization
            - L2 regularization
        * Discuss how the different models handled the various properties of the dataset
* [Day 3] Decision Trees and Random Forest
    - How Decision Tress are built?
            - The splitting process, Entropy, Information Gain, Gini Index, Chi Square
            - ID3, C4.5, C5.0, CART
            - Recursive Partitioning Tress
    - Problems with Decision Tress
        * Overfitting and instability
        * Pruning
        * Bagging and Subspace Sampling to the rescue
    - Random Forests
        * Demonstration of Random Forests counteracting overfitting
        * Training and Tuning Random Forest models in sklearn
        * Visualizing Random Forests (and feature importance)
    - Overview of Random Forest implementations
        * sklearn
        * h2o
    - [Hands-on]
        * On industry datasets, build following models
             - Logistic Regression
             - Decision Tree
             - Random Forest
        * Discuss the performance of the models in light of tha properties of the dataset
* [Day 4] More Supervised Learning Algorithms
    - Support Vector Machines
        * Hinge loss formulation (review)
        * How does SVM work?
        * Practical problems - linear separability
        * The Kernel Trick
        * What kernel to use in practice?
        * Tuning SVM models
        * Problems with SVM
    - NBC
        * brief
        * On text data
    - kNN
        * brief
        * on rent-prediction data
    - [Hands-on]
        * On industry dataset, build following models
            - SVM with linear kernel
            - SVM with polynomial kernel
            - SVM with RBF kernel
            - NBC
            - kNN
        * Discuss the performance of the models in light of the properties of the dataset
* [Day 5] Gradient Boosting Machines
    - RF to GBM
    - RF vs GBM
    - xgboost
        * GBM vs xgboost
        * early-stopping
        * hyperparameters
    - Building models and tuning with xgboost
    - xgboost with sklearn
    - Interpreting xgboost models
    - [Hands-on]
        * Participating on a Kaggle problem
        * Focus on Feature selection + xgboost + basic bagging
