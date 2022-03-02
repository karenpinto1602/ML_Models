## Building a predictor function just as linear regression but with added conditional variables too.

**Task: Build a predictor function to predict price of a home with**
* 3400 sqrt ft area in west windsor
* 2800 sqr ft home in robbinsville


### Dataset having text data
> The column town has data in text format in a categorical way.

### Approach 1
> We could convert that to a specific integer according to the category.\
> **Drawback:** This might cause the model to think that one category is ranked higher than the other(1<2<3) OR the sum of any two categories is equal to a particular category due to its numerical equivalence(1+2=3)\

#### Therefore, Categorical Variables are divided into *Nominal*(variables that do not have a numerical value or order or relationship)  and *Ordinal*(variables do have some sort of numerical ordering in between them)

##### Example
* **Nominal:** ['Green','Red','Blue'], ['Male','Female']
* **Ordinal:** ['High','Medium','Low'], ['Graduate','Masters','PHD']

\

### One Hot Encoding - For Nominal Categories
> Taking 'prices.csv' as example, for the column 'town', it will create 3 more columns viz. *monroe township*, *west windsor* and *robbinsville* and fill it with values '1' or '0'\
> These extra variables that are created are also called *Dummy Variables*
