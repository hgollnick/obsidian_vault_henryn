The best way to present and analise data with Pandas is to generalize it using ProfileReport. (More information can be found on 'Exploratory Data Analysis With Python and Pandas').

```
import pandas as pd
from pandas_profiling import ProfileReport

dataset = pd.read_csv('supermarket_sales.csv')
prof = ProfileReport(dataset)
prof
```