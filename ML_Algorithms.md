# 🧵Classification of ML
## 🔮Two types of classification
**1.** Binary Classification: Categorizing the data into 2 groups
**2.** Multi-class classification: Categorizing the data into more than 2 groups.

## 🔮Types of algorithms
- Linear Classifiers: Logistic Regression
- Tree-Based Classifiers: Decision Tree Classifier
- Support Vector Machines(SVM)
- Artificial Neural Networks
- Bayesian Regression
- Gaussian Naive Bayes Classifiers
- Stochastic Gradient Descent (SGD) Classifier
- Ensemble Methods: Random Forests, AdaBoost, Bagging Classifier, Voting Classifier, ExtraTrees Classifier

## 🔮Regression techniques
### When to use regression?
A regression problem is when the output variable is a real or continuous value, such as “salary” or “weight”. Many different models/algorithms can be used, the simplest is linear regression.
It tries to fit data with the best hyperplane which goes through the points.

*Hyperplane: is the decison boundries helps to cakssify/categorised the data points.*

### Types of regression
**- Logistic Regression**

Logistic regression measures the relationship between the categorical dependent variable (feature) and one or more independent variables (features) by estimating probabilities using a logistic function, which is the cumulative logistic distribution. 

Logistic regression is basically a **supervised classification** algorithm. In a classification problem, the target variable(or output), y, can take only discrete values for a given set of features(or inputs), X. Logistic regression is a regression model. The model builds a regression model to predict the probability that a given data entry belongs to the category numbered as “1”. Just like Linear regression assumes that the data follows a **linear function**, Logistic regression models the data using the **sigmoid function.**

**- Perceptron Algorithm**
Perceptron Algorithm consists of a set of **weights**, **input values** or **scores,threshold,net sum, and an activation function.**.
It is a building block of an **Artificial Neural Network** that helps to detect certain input data computations in business intelligence.
It is a **linear Machine Learning** algorithm used for supervised learning for various binary classifiers.
This means that it learns a decision boundary that separates two classes using a line **(called a hyperplane)** in the feature space. As such, it is appropriate for those problems where the classes can be separated well by a line or linear model, referred to as linearly separable.

The coefficients of the model are referred to as input weights and are trained using the stochastic gradient descent optimization algorithm.

Examples from the training dataset are shown to the model one at a time, the model makes a prediction, and error is calculated. The weights of the model are then updated to reduce the errors for the example. This is called the **Perceptron update rule**. This process is repeated for all examples in the training dataset, called an epoch. This process of updating the model using examples is then repeated for many epochs.

