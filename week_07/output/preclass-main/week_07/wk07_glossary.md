# Week 7 glossary

## Online resources

Documentation of xarray can be found at [https://docs.xarray.dev/en/stable/api.html](https://docs.xarray.dev/en/stable/api.html)

A good guide on color maps can be found at [https://matplotlib.org/stable/users/explain/colors/colormaps.html](https://matplotlib.org/stable/users/explain/colors/colormaps.html)

A quick guide of color maps from the `cmocean` package can be found at [https://matplotlib.org/cmocean/](https://matplotlib.org/cmocean/)

## Xarray

### Xarray functions

+ `xr.open_dataset()`: read netCDF file into an xarray Dataset object
+ `xr.Dataset.from_dataframe()`: convert a pandas DataFrame into an xarray Dataset object
+ `xr.concat()`: combine multiple Datasets or DataArrays into a single object

### Xarray Dataset/DataArray attributes and syntax

+ `<Dataset>[]`: extract a DataArray from a Dataset
+ `<Dataset>.coords[]` or `<DataArray>.coords[]`: extract coordinates of an xarray Dataset or DataArray

### Xarray Dataset/DataArray methods

+ `<Dataset>.sel()` or `<DataArray>.sel()`: subset a Dataset or DataArray by coordinate(s) value(s) of dimension(s)
+ `<Dataset>.isel()` or `<DataArray>.isel()`: subset a Dataset or DataArray by positional index(es) of dimension(s)
+ `<Dataset>.mean()` or `<DataArray>.mean()`: calculate the mean of a Dataset or DataArray along particular dimension(s)
+ `<Dataset>.median()` or `<DataArray>.median()`: calculate the median of a Dataset or DataArray along particular dimension(s)
+ `<Dataset>.min()` or `<DataArray>.min()`: calculate the minimum of a Dataset or DataArray along particular dimension(s)
+ `<Dataset>.max()` or `<DataArray>.max()`: calculate the maximum of a Dataset or DataArray along particular dimension(s)
+ `<Dataset>.sum()` or `<DataArray>.sum()`: calculate the sum of a Dataset or DataArray along particular dimension(s)
+ `<Dataset>.var()` or `<DataArray>.var()`: calculate the variance of a Dataset or DataArray along particular dimension(s)
+ `<Dataset>.std()` or `<DataArray>.std()`: calculate the standard deviation of a Dataset or DataArray along particular dimension(s)
+ `<Dataset>.squeeze()` or `<DataArray>.squeeze()`: remove coordinate(s) of size 1 from the internal array structure
+ `<Dataset>.to_dataframe()`: convert an xarray Dataset into a pandas DataFrame
+ `<Dataset>.to_netcdf()`: convert an xarray Dataset into an external netCDF file
+ `<Dataset>.expand_dims()` or `<DataArray>.expand_dims()`: add addition dimension(s) to a Dataset or DataArray
+ `<Dataset>.assign_coords()` or `<DataArray>.assign_coords()`: assign coordinates to dimension(s) of a Dataset or DataArray

### Numpy functions on Dataset/DataArray

+ `np.sqrt()`, `np.exp()`, `np.sin()`, etc.: apply numpy mapping function on DataArray

## Pandas DataFrame methods

+ `<DataFrame>.set_index()`: set particular column(s) as the index of a DataFrame
+ `<DataFrame>.reset_index()`: reset the index of a DataFrame as a regular column

## Matplotlib for 2D gridded data

+ `<Axes>.pcolormesh()`: false-color plot for 2D gridded data
+ `<Axes>.contourf()`: filled contour plot for 2D gridded data
+ `<Axes>.contour()`: line contour plot for 2D gridded data
+ `<Figure>.colorbar()`: create color bar in a figure
+ `<Colorbar>.set_label()`: set the label of the color bar
+ `<Colorbar>.ax`: obtain the Axes instance of the color bar
+ `<ContourSet>.clabel()`: create labels within the contour lines

## Color maps from the cmocean module

+ `cmocean.cm.thermal`, etc.: color maps for oceanographic data
