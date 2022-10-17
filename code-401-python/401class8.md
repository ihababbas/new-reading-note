# class 08
## Data Analysis with Pandas
import pandas as pd

Creating a Series by passing a list of values, letting pandas create a default integer index

Creating a DataFrame by passing a NumPy array, with a datetime index and labeled columns

Creating a DataFrame by passing a dictionary of objects that can be converted into a series-like structure

DataFrame.to_numpy() gives a NumPy representation of the underlying data. Note that this can be an expensive operation when your DataFrame has columns with different data types, which comes down to a fundamental difference between pandas and NumPy: NumPy arrays have one dtype for the entire array, while pandas DataFrames have one dtype per column. When you call DataFrame.to_numpy(), pandas will find the NumPy dtype that can hold all of the dtypes in the DataFrame. This may end up being object, which requires casting every value to a Python object.

describe() shows a quick statistic summary of your data

pandas primarily uses the value np.nan to represent missing data.

Operations in general exclude missing data.