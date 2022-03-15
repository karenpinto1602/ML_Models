### Just some Machine Learning stuff using sklearn


###### Training 
> ```model.fit(inputs,target) OR model.fit(inputs.values,target)```

###### Prediction
> ```model.predict(test_inputs) OR model.predict(test_inputs.values)```

###### Accuracy
> ```model.score(test_inputs,test_target)```

###### Prediction Probability
> ```model.predict_proba(test_inputs)```

###### To get a list of all the parameters to a model
> ```model.get_params(deep=True)```

###### Scale the data
> ```sklearn.preprocessing.MinMaxScaler```

> ```scaler = MinMaxScaler()``` <br/>
> ```scaler.fit(df[['Age']])``` <br/>
> ```df.Age = scaler.transform(df[['Age']])```

###### To check if any of the columns have null values
> ```data.columns[data.isna().any()]```

###### To check the total number of NANs in a column
> ```data['Column_name'].isna().sum()```

###### Using pandas to read csv
> ```import pandas as pd``` <br/>
> ```dataset = pd.read_csv('data.csv')```

###### Use datasets from sklearn
> ```from sklearn.datasets import load_iris``` <br/>
> ```dataset = load_iris()```

###### Tuning the hyperparameters
> **Use GridSearch** <br/>
> ```sklearn.model_selection.GridSearchCV```
> https://github.com/karenpinto1602/ML_Models/blob/main/Hyperparameter%20Tuning/Excercise/digitsHyperParameter.ipynb 

