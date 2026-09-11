# Week 9 glossary

## Online resources

Scipy's documentation on `linregress()` can be found at [https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.linregress.html](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.linregress.html).

For a more thorough guide of the "group-by" capability of pandas, see [https://pandas.pydata.org/docs/user_guide/groupby.html](https://pandas.pydata.org/docs/user_guide/groupby.html)

## Functions from scipy.stats

+ `scipy.stats.linregress()`: function for performing linear regression

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
  
## Matplotlib methods for multi-panel plot

+ `<Figure>.add_subplot()`: add a subplot to a matplotlib Figure instance, possibly creating a multi-panel figure.
+ `<Figure>.subplots_adjust()`: adjust the spacing between subplots of a figure
+ `<Figure>.supxlabel()`: add an overall horizontal (x-)axis label to the multi-panel figure
+ `<Figure>.supxlabel()`: add an overall vertical (y-)axis label to the multi-panel figure
+ `<figure>.suptitle()`: add an overall title to the multi-panel figure
