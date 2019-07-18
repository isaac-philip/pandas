## Pandas Basic Introduction

Pandas installation

```bash
$ pip install pandas
```

### Pandas Data Series
```python
import pandas as pd

# Pandas Series which is like a List Object with additional ability to have
#   named index
carbs = ['pizza', 'hamburger', 'rice']

carbs_ps = pd.Series(carbs)

# Output
>>> carbs_ps
0        pizza
1    hamburger
2         rice
dtype: object
```

### Pandas Data Frame
```python
# Pandas Data Frame is a two dimensional object like a table or nested dictionary which can be used to refer to data

purchase_1 = pd.Series({'Name':'Trevor', 'Ordered':'Steak','Cost':450})

purchase_2 = pd.Series({'Name':'Roger','Ordered':'Pizza','Cost':780})

purchase_3 = pd.Series({'Name':'John','Ordered':'Biryani','Cost':380})

purchase_df = pd.DataFrame([purchase_1, purchase_2, purchase_3], index=['Restaurant 1', 'Restaurant 2', 'Restaurant 3'])

# Output as Tabular format
>>> purchase_df
                Name  Ordered  Cost
Restaurant 1  Trevor    Steak   450
Restaurant 2   Roger    Pizza   780
Restaurant 3    John  Biryani   380
```


The tutorial was followed from the site below,
[Source](https://towardsdatascience.com/improve-data-quality-by-using-the-pandas-library-and-python-34fda752a6b5)