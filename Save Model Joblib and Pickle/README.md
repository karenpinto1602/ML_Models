### How to save the trained data so as to be used later again

> Pickle and Joblib can be used to save the trained model.
> Both use *dump* to save and *load* to retrive the model

#### Imports
> **Pickle: ** *import pickle* directly from python
> **Joblib: ** *import joblib* or *from sklearn.externals import joblib*

### Difference
> Although essentially it provides the same functionality, but if the model consists of large numpy arrays, then using joblib is more efficient

