## Naive Bayes Classifier Algorithm
Called Naive because here naive assumptions are made that the features are independed of each other.

### Probability
> P(A/B) = Probability of event A knowing that event B has already occured

> Thomar Bayes conditional probability equation states <br />
 **P(A/B) = [P(B/A)*P(A)] / [P(B)]** 

 ### Naive Bayes Classifiers
 1. **Bernoulli:**  It assumes that all our features are binary such that they take only two values. Means 0s can represent *word does not occur in the document* and 1s as *word occurs in the document.*
 2. **Multinomial:** It is used when we have discrete data(Eg. movie ratings ranging from 1 to 5 as each rating will have certain frequency to represent). In text learning we have the count of each word to predict the class or label.
 3. **Gaussian:** Assumes Normal distribution. This is used in cases when all our features are continous. For example, in the iris dataset features are sepal width, petal width, sepal length and petal length. So its features can have different values in the dataset as width and length can vary. We can't represent features in terms of their occurences. This means data is continous. Hence we use Guassian Naive Bayes here. 

 ### Imports
 > **Guassian** <br/>
 ```sklearn.naive_bayes.GaussianNB```

 > **Multinomial** <br/>
 ```sklearn.naive_bayes.MultinomialNB```

 ### CountVector - to create a frequency metrics
 > ```from sklearn.feature_extraction.text import CountVectorizer``` <br/>
 ```v = CountVectorizer()``` <br/>
 ```x_train_count = v.fit_transform(x_train.values)``` 

 ### Pipeline - alternative to the above, works as an all in one function
 > ```from sklearn.pipeline import Pipeline``` <br/>
 ```clf = Pipeline([('vectorier', CountVectorizer()),('nb',MultinomialNB())])```