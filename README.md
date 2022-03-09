### Just some Machine Learning stuff using sklearn




###### To get a list of all the parameters to a model
> ```model.get_params(deep=True)```

###### Scale the data
> ```sklearn.preprocessing.MinMaxScaler```

> ```scaler = MinMaxSCaler()```
> ```scaler.fit(df[['Age']])```
> ```df.Age = scaler.transform(df[['Age']])```
