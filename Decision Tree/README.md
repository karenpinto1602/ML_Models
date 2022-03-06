## Decision Tree

When the feautres need to be divided at every stage to get the result.

### How to select the ordering of features 
> Select the one that produces a category or split section with low entropy(randomness)

### Library from sklearn
> ```sklearn.tree.DecisionTreeClassifier```

### Difference between Gini and Entropy
> ```criterion='gini'```

> Gini Index has values inside the interval [0, 0.5] whereas the interval of the Entropy is [0, 1].

> Gini Impurity is better as compared to entropy for selecting the best features.