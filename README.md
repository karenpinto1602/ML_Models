### Just some Machine Learning stuff using sklearn


###### Training 
> model.fit(inputs,target)

###### Accuracy
> model.score(test_inputs,test_target)

###### Prediction Probability
> model.predict_proba(test_inputs)

###### To get a list of all the parameters to a model
> ```model.get_params(deep=True)```

###### Scale the data
> ```sklearn.preprocessing.MinMaxScaler```

> ```scaler = MinMaxSCaler()``` <br/>
> ```scaler.fit(df[['Age']])``` <br/>
> ```df.Age = scaler.transform(df[['Age']])```

###### To check if any of the columns have null values
> ```data.columns[data.isna().any()]```

###### To check the total number of NAs in a column
> ```data['Column_name'].isna().sum()```


