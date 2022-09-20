![housesbanner](https://user-images.githubusercontent.com/98269318/191279386-02ca09a5-dfbf-4d95-8b3d-537b5b060531.png)
# Machine-Learning-House-prediction

## 🖥️Purpose of this prediction
**1.** Finding & removing the outliers

**2.** Relation between overall quality of the house & Sales Price

**3.** Relation between grade living area & Sales Price

**4.** Relation between Garage area & Sales Price

**5.** Relation between Basement area & Sales Price

**6.** Relation between First floor & Sales Price

**7.** Relation between total bath rooms & Sales Price

**8.** Relation between Total rooms & Sales Price

**9.** Relation between Orignal construction year & Sales Price

**10.** Calculating Mean Absolute Error, Mean Square Error,& Root Mean Square Calculation by Decision Tree Regresion, Random Forest Regressor & Light Gradient Boosting.

# 💡How I approched to solve this dataset
**1.** Importing libraries from  for dataframe 
``` python
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
import warnings
warnings.filterwarnings('ignore')
sns.set(style='white', context='notebook', palette='deep')
%config InlineBackend.figure_format = 'retina' #set 'png' here when working on notebook
%matplotlib inline
```
**2.** Importing Libraries for machine learning
``` python
from sklearn.linear_model import LogisticRegression, LinearRegression
from sklearn.model_selection import cross_val_score
from sklearn.ensemble import RandomForestRegressor
from sklearn.preprocessing import StandardScaler
from sklearn.model_selection import train_test_split
from sklearn import metrics
from sklearn import ensemble
from sklearn.utils import shuffle
from sklearn.metrics import mean_squared_error, r2_score
from sklearn.tree import DecisionTreeRegressor
import lightgbm as lgb
```

