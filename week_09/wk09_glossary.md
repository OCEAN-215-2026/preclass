# Week 9 glossary

## Online resources

For a more thorough guide of the "group-by" capability of pandas, see [https://pandas.pydata.org/docs/user_guide/groupby.html](https://pandas.pydata.org/docs/user_guide/groupby.html)


## Pandas group summarization methods

+ `<DataFrame>.groupby()`: group rows of a DataFrame for summarization. The result is a pandas DataFrameGroupBy object
+ `<DataFrameGroupBy>.count()`: count the number of non-NA values in each group
+ `<DataFrameGroupBy>.max()`: Compute the maximum value in each group
+ `<DataFrameGroupBy>.min()`: Compute the minimum value in each group
+ `<DataFrameGroupBy>.mean()`: Compute the mean of each group
+ `<DataFrameGroupBy>.median()`: Compute the median of each group
+ `<DataFrameGroupBy>.nunique()`: Compute the number of unique values in each group
+ `<DataFrameGroupBy>.quantile()`: Compute a given quantile of the values in each group
+ `<DataFrameGroupBy>.sem()`: Compute the standard error of the mean of the values in each group
+ `<DataFrameGroupBy>.std()`: Compute the standard deviation of the values in each group
+ `<DataFrameGroupBy>.var()`: Compute the variance of the values in each group
+ `<Series>.astype()`: coerce the conversion of data type of a pandas series
