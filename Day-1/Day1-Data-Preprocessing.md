# Data Preprocessing

### Prerequisite
In this section, you can download the following material, and use the language to learn the concept:

- Python:
[Data-Preprocessing-Python](/Day-1/course-material/Data-Preprocessing-Python.zip)

- R:
[Data-Preprocessing-R](/Day-1/course-material/Data-Preprocessing-R.zip)

### Import Library
``` python
import numpy as np
import matplotlib.pyplot as pit
import pandas as pd
```

### Importing the dataset
``` python
# ensure your dataset file is import into the codelab
dataset = pd.read_csv('Data.csv') 

# get all the data exclude the last column
x = dataset.iloc[:, :-1].values 

# get the last column data
y = dataset.iloc[:, -1].values 

# Check x and y values
print(x)
print(y)
```

### Taking care of missing data
There two method to replace the missing data here.
1. We ignore the missing data since the data only contain a tiny percentage, such as 1%, which won't affect the entire dataset.

2. We can use the average of values to replace the missing values.

```python
from sklearn.impute import SimpleImputer

# replace the missing values with the average values.
imputer = SimpleImputer(missing_values=np.nan, strategy='mean')
imputer.fit(x[:, 1:3])
x[:, 1:3] = imputer.transform(x[:, 1:3])
```
---
Next &rarr; []()
\
Previous &larr; [Feature Scaling](/Day-1/Day1-Feature-Scaling.md)