# Week 6 glossary

## Online resources

The official pandas documentation page is at [https://pandas.pydata.org/docs/reference/index.html](https://pandas.pydata.org/docs/reference/index.html).

The documentation of `matplolib.dates` submodule is at [https://matplotlib.org/stable/api/dates_api.html](https://matplotlib.org/stable/api/dates_api.html)

## Internet download functions

+ `urlretrive()` (from `urllib.request`): retrieve a file from the internet to the local file system.
+ `gdown.download()`: download a public Google Drive file to the local file system
+ `zipfile.Zipfile()`, `<Zipfile>.extractall()`: extract the content of a zip file.

## Pandas functions

+ `pd.DataFrame()`: create a new DataFrame manually
+ `pd.read_csv()`: reading a csv file into a DataFrame
+ `pd.read_excel()`: reading an Excel file into a DataFrame
+ `pd.isna()`: vectorized check on which values are missing
+ `pd.to_datetime()`: convert strings to datetime objects
+ `pd.Series()`: create a pandas Series from arrays or pandas indices

## Pandas DataFrame attributes

+ `<DataFrame>.size`: the size (number of entries) of the DataFrame
+ `<DataFrame>.shape`: the shape (number of rows, columns) of the DataFrame
+ `<DataFrame>.ndim`: the number of dimension of the DataFrame
+ `<DataFrame>.columns`: the column names of the DataFrame
+ `<DataFrame>.index`: the index (row labels) of the DataFrame

## Pandas DataFrame methods

### DataFrame manipulation

+ `<DataFrame>.info()`: print out summary information about the DataFrame
+ `<DataFrame>.iloc[]`: subset the DataFrame by row and column indices
+ `<DataFrame>.loc[]`: subset the DataFrame by row and column labels
+ `<DataFrame>.dropna()`: dropping rows with missing values from the DataFrame
+ `<DataFrame>.sort_index()`: sort the rows of a DataFrame by the values of its index
+ `<DataFrame>.sort_values()`: sort the rows of a DataFrame by values from certain columns
+ `<DataFrame>.reset_index()`: reset the index of a DataFrame as a regular column
+ `<DataFrame>.set_index()`: set a column of the DataFrame as the DataFrame's row index
+ `<DataFrame>.to_csv()`: export a DataFrame as an external csv file

### Descriptive statistics

+ `<DataFrame>.describe()`: compute multiple descriptive statistics for all columns of a DataFrame all at once
+ `<DataFrame>.mean()`: compute the mean for all columns of a DataFrame
+ `<DataFrame>.median()`: compute the median for all columns of a DataFrame
+ `<DataFrame>.quantile()`: compute a given quantile for all columns of a DataFrame
+ `<DataFrame>.var()`: compute the variance for all columns of a DataFrame
+ `<DataFrame>.std()`: compute the standard deviation for all columns of a DataFrame
+ `<DataFrame>.sem()`: compute the standard error for all columns of a DataFrame

## Pandas datetime Series attributes and methods

+ `<Series>.dt.strftime()`: produce datetime strings from datetime Series
+ `<Series>.dt.year`: extract the years of the datetime Series
+ `<Series>.dt.month`: sxtract the months of the datetime Series
+ `<Series>.dt.day`: extract the days of the datetime Series
+ `<Series>.dt.hour`: extract the hours of the datetime Series
+ `<Series>.dt.minute`: extract the minutes of the datetime Series
+ `<Series>.dt.dayofyear`: extract the days of year of the datetime Series

## Datetime plotting utilities from `matplotlib.dates`

+ `mdates.YearLocator()`: place ticks on year-level intervals
+ `mdates.MonthLocator()`: place ticks on month-level intervals
+ `mdates.DayLocator()`: place ticks on day-level intervals
+ `mdates.HourLocator()`: place ticks on hour-level intervals
+ `mdates.MinuteLocator()`: place ticks on minute-level intervals

