> **Update:** Section 5 of this talk concerning Model Explainability and Interpretability  were also covered in the Kaggle NYC Meetup held on 03/27/19 at Deliotte Digital. 

# Applied Machine Learning Workshop, 02/28/2019

![Workshop Poster](/fig/workshop_poster.jpg)

This is the notebook from the [Columbia Data Science Society's](https://www.facebook.com/cdsscu/) Workshop on [**Applied Machine Learning**](https://www.facebook.com/events/247226822888651/).

**Presented by:** Akhil Punia, MS Data Science (2019)

## Acknowledgement
The content of this talk is motivated from the two classes, I am taking this semester at Columbia Data Science Institute.

- [COMS W4995 Applied Machine Learning ](http://www.cs.columbia.edu/~amueller/comsw4995s19/schedule/) taught by **AndreaS C. Müller**, core contributer of sci-kit learn and author of the O'Reilly book "Introduction to machine learning with Python", describing a practical approach to machine learning with python and scikit-learn. 

- [COMS W4721 Machine Learning for Data Science](http://www.columbia.edu/~jwp2128/Teaching/W4721/Spring2019/W4721Spring2019.html) taught by **Prof. John Paisley**. He also teaches a course on [**Machine Learning**](https://www.edx.org/course/machine-learning-columbiax-csmm-102x-0) through **edx**.The content of his on-campus course largely overlaps with his edx class.


## How to Run the Notebook ?

1. Go to https://colab.research.google.com/
2. Select the Github Tab and add the repository from the search bar.

![Connect Notebook](/fig/connect_nb.png)

3. Click on **Connect** on the upper right hand corner. And off you go.

![Baic Notebook View](/fig/basic_nb.png)

## Basic Outline of the Notebook

#### 01 Dataset: House Prices Regression [70%]
  - 1.1 : EDA : 
    - Categorical 
    - Continous 
    - *Ordinal
  - 1.2 : Treat Missing Values
    - sklearn impute
    - encoding for missing values 
  - 1.3 : Outliers
  - 1.4 : Feature Engineering
    - Polynomial Featues
    - Label Encodings
 
> Q: How do you clean your data and look for patterns ?

#### 02 Models: [10%] 
  - 2.1 : Linear Regression: l1, l2, elastic net
  - 2.2 : Logistic Regression
  - 2.3 : Decision Trees
    - 2.3.1: Random Forest
    - 2.3.2: Bagging
    - 2.3.3: Gradient Boosting: xgboost ( others: lightgbm,  catboost)

> Q: What are the two main class of machine learning models?

#### 03 Model Evaluation and Improvement ( aka Parmeter Tuning ) [20%]
  - 3.1 : Metrics: Accuracy, Precision, Recall, F-Score , [ MAPE ( forecasting ) ]
  - 3.2 : Plots:  ROC, Confusion Matrix, Prediction Plots, Residual Plots, Residuals vs Features Plot
  - 3.3 : Hard Coded Optimization: GridSearch, RandomSearch
  - 3.4 : New Techniques: ( skopt, bayesian opt, hypreropt )
  
> Q: How do you check if your regression model is giving reasonable conditions ?

#### 04 Special Challenges: 
  - 4.1 Ovefitting
    - 4.1.1 : Train, Test, Valid
    - 4.1.2 : Regularisation
  - 4.2 : Class Imbalance: 
    - 4.2.1 : Problem Description
    - 4.2.2 : Possible Solutions ( Under and Over Sampling, Loss Fucntions )

> Q: What is better Type-I or Type II error ( a.k.a. False Positives and False Negatives ) ? 

#### 05 Model Explanability
  - Feature Importance  
  - Regression Coefficients
  - XGBoost Feature Importance
  - New Stuff: Impact of Individual Predictions
    - SHAP Values
> Q: How do you find out which features are the most important ?

#### 06 Resources
  - Kaggle: Regression Challenge ( House Prices ): https://www.kaggle.com/c/house-prices-advanced-regression-techniques
  - Kaggle: Machine Learning Explainability: https://www.kaggle.com/learn/machine-learning-explainability
  - Categorical Data Plotting: https://seaborn.pydata.org/tutorial/categorical.html
  - Continous Data Plotting: https://seaborn.pydata.org/tutorial/distributions.html#plotting-univariate-distributions
  - sklearn: https://scikit-learn.org/stable/
  - xgboost: https://xgboost.readthedocs.io/en/latest/
  - yellowbrick: https://www.scikit-yb.org/en/latest/index.html
  - skopt: https://scikit-optimize.github.io
  - bayesianopt: https://github.com/fmfn/BayesianOptimization
  - hyperopt:https://github.com/hyperopt/hyperopt
  - eli5: https://eli5.readthedocs.io/en/latest/index.html
  - shap: https://github.com/slundberg/shap
  
#### 07 Quick Tips
  - Code Breaks: Library Version , pip/ conda upgrade -> virualenv
  - Visualising High Dimensional Data: Principal Component Analysis
