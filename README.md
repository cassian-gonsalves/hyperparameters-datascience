# AI Skunkworks Project - Hyperparameters Database

#### Goals and Objectives :
<ul>
<li>In statistics, hyperparameter is a parameter from a prior distribution; it captures the prior belief before data is observed.</li>
<li>In any machine learning algorithms, these parameters need to be initialized before training amodel.</li>
<li>Hyperparameters are important because they directly control the behaviour of the training algorithm and have a significant impact on the performance of the model is being trained.</li>
<li>Our aim is to find proper hyperparameter with proper tuning for our dataset which would help the database team in modelling the database schema in an efficient way. We would create H2O models for this dataset for getting proper hyperparameters.</li>
</ul>

#### Background Research:
Hyperparameters are variables that we need to set before applying a learning algorithm to a dataset. In machine learning scenarios, a significant part of model performance depends on the hyperparameter values selected. The goal of hyperparameter exploration is to search across various hyperparameter configurations to find the one that results in the optimal performance.  The challenge with hyperparameters is that there are no magic number that works everywhere. The best numbers depend on each task and each dataset. The hyperparameter database to be developed as a part of this project is an open resource with algorithms, tools, and data that allows users to visualize and understand how to choose hyperparameters that maximize the predictive power of their models. Phase I of the project involves selecting a unique dataset containing predicted target variables, hyperparameters, meta-data etc. by running different models (with varying hyperparameters) on it using H2O.<br>

**Hyperparameters can be divided into 2 categories:** <br>
1. Optimizer hyperparameters
<ul>
<li>They are related more to the optimization and training process</li>
<li>If our learning rate is too small than optimal value then it would take a much longer time (hundreds or thousands) of epochs to reach the ideal state</li>
<li>If our learning rate is too large than optimal value then it would overshoot the ideal state and our algorithm might not converge</li>
</ul><br>

2. Model Specific hyperparameters
<ul>
<li>They are more involved in the structure of the model</li>
</ul>

Currently, the hyperparameter database analyzes the effect of hyperparameters on the following algorithms: Distributed Random Forest (DRF), Generalized Linear Model (GLM), Gradient Boosting Machine (GBM). Naïve Bayes Classifier, Stacked Ensembles, XGBoost and Deep Learning Models (Neural Networks).


**Algorithms and code sources:**
<ul>
<li>Deciding the algorithms based on the type of dataset(Classification or Regression algorithm)</li>
<li>We would be using H20 python module.</li>
<li>This Python module provides access to the H2O JVM, as well as its extensions, objects, machine-learning algorithms, and modeling support capabilities, such as basic munging and feature generation. </li>
</ul>
    
**How and what the team will work on?:**
<ul>
<li>Find a dataset</li>
<li>Figure out the algorithms that will work for that dataset. The type of algorithm like classification or Regression algorithm.</li>
<li>Perform H2O in python for generating various models at various runtime.</li>
<li>Suppose hypothetically if five algorithms are used then the best models for those algorithms will be selected to get the hyperparameter.</li>
<li>All the models will be stored for reference irrespective of it being best or the worst model.</li>
<li>Further communicate with the database team to give them the insight of the data and the conclusions drawn from the H2O analysis. This would help them in designing the ER Diagrams and designing the data models and schema.</li>
<li>We will try to follow this process on as many datasets as possible within the given time constraint.</li>
</ul>
    
**Challenges:**
<ul>
<li>Implementing H2O analysis.</li>
<li>Getting optimized hyperparameters.</li>
<li>The model might overfit for the training dataset which will not work well on the test dataset.</li>
<li>Other challenge would be to tune model and feature parameters well.</li>
</ul>
