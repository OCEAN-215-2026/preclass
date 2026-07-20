# Week 4 glossary

## Online resources

The official numpy documentations can be found at [https://numpy.org/doc/stable/reference/index.html#reference](https://numpy.org/doc/stable/reference/index.html#reference). You may find the page of array creation routines ([https://numpy.org/doc/stable/reference/routines.array-creation.html](https://numpy.org/doc/stable/reference/routines.array-creation.html)) and mathematical functions ([https://numpy.org/doc/stable/reference/routines.math.html](https://numpy.org/doc/stable/reference/routines.math.html)) especially useful.

## Numpy syntax

### arithmetic

+ `+`, `-`, `*`, `/`, `//`, `%`, `**`: vectorized arithmetic operators between 2 numpy arrays or between a numpy array and a scalar.

### logical comparison

+ `==`, `!=`, `<`, `>`, `<=`, `>=`: vectorized comparison operators between 2 numpy arrays or between a numpy array and a scalar.
+ `~`: vectorized negation on a numpy boolean array
+ `&`, `|`: vectorized "and" and "or" between two numpy boolean arrays

### Array indexing

+ `[]`: indexing operator on numpy arrays
+ `:`: create basic slicing of the form _start_:_stop_:_step_

## Numpy constants

+ `np.e`: the natural / Euler / exponential number
+ `np.pi`: the number $\pi$
+ `np.nan`: the "not a number" value<br><br>

+ `np.isnan()`: check if a value is `np.nan`

## Numpy array attributes

+ `<ndarray>.size`: the size (number of entries) of a numpy array
+ `<ndarray>.shape`: the shape of a numpy array
+ `<ndarray>.ndim`: number of dimensions of the numpy array

## Numpy functions

### Array creation

+ `np.array()`: create an array from a python list
+ `np.linspace()`: create a linearly-spaced array of $n$ elements from $a$ to $b$ ($b$ inclusive)
+ `np.arange()`: create an evenly-spaced array from $a$ to $b$ ($b$ exclusive) at steps of $d$
+ `np.zeros()`: create an array of zeros
+ `np.ones()`: create an array of ones
+ `np.full()`: create a constant array
+ `np.concatenate()`: concatenate two numpy arrays into one

### Mapping functions

+ `np.sqrt()`:  square root
+ `np.exp()`: exponentiation
+ `np.log()`: natural logarithm
+ `np.log10()`: base-10 logarithm
+ `np.log2()`: base-2 logrithm<br><br>

+ `np.sin()`, `np.cos()`, `np.tan()`: trigonometric functions
+ `np.arcsin()`, `np.arccos()`, `np.arctan()`: inverse trigonometric functions
+ `np.arctan2()`: arctangent function accepting both `x` and `y` as arguments
+ `deg2rad()`, `rad2deg()`: conversion between radians and degrees<br><br>

+ `np.round()`: round values to fixed decimal point
+ `np.floor()`: round *down* to the nearest integer
+ `np.ceil()`: round *up* to the nearest integer<br><br>

+ `np.fabs()`: absolute value

### Reduction functions

+ `np.mean()`: calculating average
+ `np.var()`: calculating variance
+ `np.std()`: calculating standard deviation
+ `np.median()`: calculating median
+ `np.quantile()`: calculating quantiles<br><br>

+ `np.prod()`: product over elements
+ `np.sum()`: sum over elements<br><br>

+ `np.max()`, `np.min()`: finding extremum *value* of an array
+ `np.argmax()`, `np.argmin()`: finding the *index* at which the extremum is attained<br><br>

+ `np.nanmean()`, `np.nanmedian()`, `np.nanvar()`, `np.nanstd()`, `np.nanmin()`, `np.nanmax()`, `np.nansum()`: "nan-omitted" variation of the respective functions without the `nan` in their names

### Other functions

+ `np.sort()`: sort an array
+ `np.argsort()`: sort the index of an array by the corresponding values


