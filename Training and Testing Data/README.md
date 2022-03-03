## Methods used to split datasets into training and testing set

> ***using sklearn.model_selection.train_test_split*** 

#### When splitting the datset into training and testing
* **shuffle=False** - the spilted sets will be in order if the dataset is already in order else if True, it will be randomly divided
* **random_state=None** - everytime the code is run, it will generate a randomly shuffeled set.
* **random_state=0 or any other integer** - everytime the code is run, it will give the same shuffled(if True or not mentioned) set of training and testing dataset.
* If the dataset is not already ordered, and needs to be done according to a time series then refer, https://stackoverflow.com/questions/50879915/splitting-data-using-time-based-splitting-in-test-and-train-datasets 