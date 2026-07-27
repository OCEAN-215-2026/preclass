# Installing additional python packages

In some rare cases, the final project you pursue may lead you to a python package (a.k.a. third-party modules) that is not included in our JupyterHub environment or in the local python environment set up through the instruction in the "Installing python locally" appendix. In such cases, it is possible to install the extract package manually. And we describe how to do so for both JupyterHub and local python environment below.

## Installing packages on JupyterHub

Suppose that my final project somehow requires Markov chain Monte Carlo via the [PyMC](https://www.pymc.io/welcome.html) package. At the top of the notebook from which the simulation is to be run, insert a code cell, and put in the following:

```python
!pip install -U pymc
```

Run this code cell as usual (i.e., with `Shift` + `Enter`), and you will see python doing the work of installing the packages and its dependencies. You can then import this package as usual in your code, e.g.,

```python
import pymc
```

After which you can access the functions in the module using the usual `pymc.<name>` syntax.

To install and use other packages, just replace `pymc` in the above lines with the name of the package you need.

Unfortunately, due to the underlying architecture of JupyterHub, packages installed this way are not permanently retained. So to be safe, you will have to re-run the `!pip` line everytime you need to run the codes of your custom package.

## Installing packages on local python

In comparison, you can permanently install a package in your local python environment. To do so, open a mamba-enabled terminal and activate the environment that corresponds to this course (if you follow the "Installing python locally" appendix, this will be the `learn` environment). Now, if your package is available on conda-forge (which you can check via [this page](https://conda-forge.org/packages/)), it is perferable to use `mamba` to install the package. Using our example, it turns out that `pymc` is available on conda-forge, so to install I will need to execute:

```
mamba install pymc
```

Mamba will then figure out what packages need to be installed, and once you confirm the changes the package will be installed to your environment and available for all future use. In other words, when you run your jupyter notebook in the `learn` environment, the pymc package will be available via `import pymc`.

If your package is not available on conda-forge it is likely distributed via pypi. Such packages can be installed using `pip`. For example, if I want to install PyMC via `pip`, I will have to run:

```
pip install -U pymc
```

(Note that if your package is available on conda-forge and you've already run the `mamba install` line then you **do not** need to perform `pip install`. In any case, only one of the two lines are needed).

As with `mamba install`, the new package is now permanently a part of your python environment and you all you need to do to use it in a notebook is to import the package.

To install and use other packages, again just replace `pymc` in the above lines with the name of the package you need.