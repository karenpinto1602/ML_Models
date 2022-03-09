## K Fold Cross Validation

Cross Validation is a technique which allows us to evaluate a model performance or decide which among the various ways is the best suited one. 

### Different Ways to perform the training step
1.  Use all available data for training and testing on the same dataset.  

*Issue here is that it might give a 100% accuracy because we aren't testing a new diff type of inputs*

2. Split the sample into training and testing - ```sklearn.model_selection.train_test_split```
   
*Issue here is that while dividing what if a particular unique set of inputs is put under testing, then the model would not have seen such a type of question or something to make a prediction*

3. K fold cross validation - here we divide our samples into n folds

Then n iterations are run, at each iteration one fold is used for testing and the remaining for training. This way every fold takes part in the testing. 

At the end, the average of all the scores predicted at each iteration is taken and is produced as the final outcome. 

### Imports
> ```sklearn.model_selection.KFold```

**OR**

> ```klearn.model_selection.StratifiedKFold```

**Along with parameters**

> ```kf = KFold(n_splits=3) # specifies 3 folds```

These two methods can then be used with for loops to display the scores or use the below library that is a combined function of the above

> ```sklearn.model_selection.cross_val_score``` this will return an array of scores

> ```cross_val_score(model,data_input,data_output,cv=3)``` this produces 3 folds, thereby giving an array with 3 accuracy scores

### Refer Excercise 