## Titanic_Survivers_Predictions
### Objectives 
- Cleaning the dataset with the help of libraries like pandas and numpy
- Visualizing the dataset with matplotlib & seaborn
- Predicting the highest accurcy of the model by machine learning algorithms

### Libraries used for data frame and visualizations
- numpy
- pandas
- matplotlib.pyplot
- seaborn

### ML algorithms I used for modeling & predicting
- Logistic regression
- Linear SVC
- Decision Tree Classifier
- K-Neighbour Classifier
- Random Forest Classifier
- SGD Classifier
- Perceptron

### How I soved the dataset
- Claculated the passenges survival rate with different categories- Pclass, Embarked, SibSp & Parch by using the function **mean & group by**.
- Dropped the **Ticket & Cabin** coulumns by using the feature **drop** because it has ni use in further predictions and visualizations
- Extracted the Titles form the column **Name** by using the function **str.extract**, replaced all the titles with Miss, Ms, Mr, Master & Rare and then calculated its survival rate. After replacing converted the column from string to numeric format for implenting ML algorithms(ML algorithms only work in numeric data-type: int, float, double)
- Now column **Title** has been converted to numeric data-type, dropped the column **Name & PassengerId** as it will be not required for further analysis.
