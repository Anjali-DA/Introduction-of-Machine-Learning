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

## 🖥️How I approched to solve this dataset
💡 **Importing libraries from  for dataframe** 
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
**Importing Libraries for machine learning**
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
- Dropping 'Id' from train & test data because it is not necessary for further analysis & prediction.
- Creating/selecting **int** data type columns into train_df & test_df.

## 🖥️ Finding correlation & outliers

- For finding the correlation I used seaborn **barplot** & **jointplot**.
- To remove the outliers I used drop & reset_index function.

💡 **Relation between Overall house quality and Sales price**

**Output:** 
- In this correlation, Overall quality of the house increases with increase in price
- There are no outliers as both of the features increases proportionally.

💡 **Relation between Ground living area and Sales price**

**Output:**
In this correlation, with increase in ground living area, Sales price also increases but I spotted two points where increase in ground living area, sales price decreases.Hence, There are outliers and I have removed them by using drop function.
<img width="449" alt="__results___23_1" src="https://user-images.githubusercontent.com/98269318/191994496-22471d8c-f239-44a3-9bc3-62bc6ead0fb6.png">
*pic-1: correlation with outliers*

<img width="449" alt="__results___20_1" src="https://user-images.githubusercontent.com/98269318/191994543-30bee187-c590-4d7a-8304-1291e999d941.png">

*pic-2: correlation without outliers*

💡 **Relation between Garage cars & Sales price**
In this correlation, with increase in garage capacity, sales price also increases, but I spotted a bar where garage capacity increases with decrease in sales price which doesn't seem fit in this analysis.

<img width="417" alt="__results___25_0" src="https://user-images.githubusercontent.com/98269318/192113087-63d8c8e8-22b8-40e0-8157-bf01f159480f.png">
