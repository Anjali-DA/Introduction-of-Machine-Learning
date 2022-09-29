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
