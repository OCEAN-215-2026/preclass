# Week 5 glossary

## Online resources

The official matplotlib documentation can be found in [https://matplotlib.org/stable/api/index.html](https://matplotlib.org/stable/api/index.html) (*note*: we are using the "axes interface")

In addition, you may find the cheatsheets provided by matplotlib ([https://matplotlib.org/cheatsheets/](https://matplotlib.org/cheatsheets/)) useful.

## Numpy syntax

+ `+`, `-`, `*`, `/`, `//`, `%`, `**`: arithmetic operators on multi-dimensional numpy arrays`<br><br>`
+ `[]`: indexing operators on multi-dimensional numpy array
+ `:` : operator to create slicing object of form _start_:_stop_:_step_

## Numpy attributes, functions and methods

## Numpy array attributes

+ `<ndarray>.size`: the size (number of entries) of a numpy array
+ `<ndarray>.shape`: the shape of a numpy array
+ `<ndarray>.ndim`: number of dimensions of the numpy array

### Numpy array methods

+ `<ndarray>.reshape()`: reshape an numpy array
+ `<ndarray>.flatten()`: flatten a multi-dimensional array to 1D
+ `<ndarray>.transpose()`: transpose the rows and columns of a 2D numpy array

### Numpy array combining functions

+ `np.concatenate()`: concatenate numpy arrays along a specified axis
+ `np.vstack()`: combine 2D numpy arrays vertically (i.e., extending rows)
+ `np.hstack()`: combine 2D numpy arrays horizonatal (i.e., extending columns)

### Numpy mapping functions

+ `np.exp()`, `np.sin()`, etc. Functions that applying a mapping to each element of a multi-dimensional array (for a more complete list, see the glossary of week 4)

### Numpy reduction functions

+ `np.mean()`, `np.sum()`, etc. Functions that apply reduction along particular axis / axes or across the whole multi-dimensional array (for a more complete list, see the glossary of week 4)

## matplotlib functions

### Creating, showing, and exporting figures and axes

+ `plt.figure()`: create a new figure
+ `<Figure>.add_subplot()`: add new axes object to a Figure instance
+ `<Figure>.savefig()`: save a figure to an external file
+ `plt.show()`: show a figure already created

### Making different types of visualization

+ `<Axes>.plot()`: create a line plot on an Axes instance
+ `<Axes>.scatter()`: create a scatter plot on an Axes instance
+ `<Axes>.errorbar()`: create an error bar plot on an Axes instance
+ `<Axes>.bar()`: create a bar plot on an Axes instance
+ `<Axes>.hist()`: create a histogram on an Axes instance
+ 
### Axes and titles

+ `<Axes>.set_title()`: set the title of the figure, for an Axes instance
+ `<Axes>.set_xlabel()`, `<Axes>.set_ylabel()`: set the labels for x- and y-axis, respectively, for an Axes instance
+ `<Axes>.set_xlim()`, `<Axes>.set_ylim()`: set the x- and y-axis limits, respectively, for an Axes instance
+ `<Axes>.set_xticks()`, `<Axes>.set_yticks()`: set the ticks for x- and y-axis, respectively, for an Axes instance
+ `<Axes>.tick_params()`: set the parameters for ticks (e.g., font size for tick labels), for an Axes instance
+ `<Axes>.grid()`: create a grid overlay for an Axes instance
+ `<Axes>.legend()`: create a legend for an Axes instance
