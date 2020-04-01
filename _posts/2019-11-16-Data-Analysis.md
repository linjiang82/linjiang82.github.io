The best way to drop non-numeric column from a DF?
 import numpy as np
 df.select_dtypes(include=[np.number])
 
astype to change the type
value_counts
df.isnull() df.notnull()
df.dropna(how='any') df.fillna() //handle missing value
df.sample(n=3,ramdon_state=42) df.sample(frac=0.75) //Reduce the dataset size
map() //
pd.get_dummies()
df.duplicated(keep=False)
pd.describe_option()
apply(max,axis=0) or apply(np.argmax, axis =0 )
pivot_table()
// multiindex
// during file reading, can create a category

Date time handling
 Using python built-in datetime library to create datetime type data, and using that data  can distill any format date or time. [link](https://jakevdp.github.io/PythonDataScienceHandbook/03.11-working-with-time-series.html)
