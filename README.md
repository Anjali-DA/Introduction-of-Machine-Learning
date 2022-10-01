![housesbanner](https://user-images.githubusercontent.com/98269318/191279386-02ca09a5-dfbf-4d95-8b3d-537b5b060531.png)
# Machine-Learning-House-prediction

## 🖥️Purpose of this prediction
**1.** Finding correlation with sales price and outliers.

**2** Filling up the missing data in the train dataset

**3** Fitting & transforming the test & train data

**4** Predicting the dataset in linear regression, Random forest regression, Decision tree regression, Light gradient boosting.

## 🖥️ How I approached to solve this dataset
- Imported the libraries and datasets
- Dropped 'Id' column as it is unnecessary for the prediction.
- Created test_df and train_df to do the supervised learning with this datasets.
- Found the most correlated features by using *corr* feature.
- Found the outliers and relations between correlated features and Sales price.
- By using *.isnull().sum().sort_values()*, I found the missing values in train & test data.
- Splitted the dataset into train and test with *train_test_split* 
- Reshaped the train & test dataset with *reshape(-1,1)*
- With *StandardScaler*, I transofermed the data into fit data. *StandardScaler* is also called as a Feature scaling, if it is not done, then a ML algorithm tends to weigh greater values, higher and consider smaller values as the lower values, regardless of the unit of the values.
- With *LinearRegression()* , *RandomForestRegressor()*  , *LGBRegressor()* (Light Gradient Boosting), I calculated the **MAE(Mean Absolute error)**, **MSE(Mean Square Error)** & **RMSE(Root Mean Square Error)**. 

**Values calculated with Linear Regression**:

![linear](https://user-images.githubusercontent.com/98269318/193422748-5593fafa-7c60-4d17-8ef1-6ef0dd7dbd7c.png)

**Values calculated with Random Forest Regression**:

![random](https://user-images.githubusercontent.com/98269318/193423329-78c924f3-2d9b-465d-a3a2-a9ad448ec499.png)

**Values calculated with Light Gradient Boosting Regression**:

![light](https://user-images.githubusercontent.com/98269318/193423372-7b1b8b29-d6b7-4906-8800-6753559499d0.png)
