
# Package Intro
A package contains one or more relevant modules, which can be interlinked with each other.

A directory with subdirectories can be called a package if it contains a __init__.py file.

## Example Package Structure 

|-Folder: Package_A
|&nbsp;&nbsp;&nbsp;&nbsp;|-file: \__init__.py
|&nbsp;&nbsp;&nbsp;&nbsp;|-file: f1.py
|&nbsp;&nbsp;&nbsp;&nbsp;|-file: f2.py
|&nbsp;&nbsp;&nbsp;&nbsp;|-Folder: Sub_package_A
|&nbsp;&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;&nbsp;|-file: \__init__.py
|&nbsp;&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;&nbsp;|-file: f3.py
|&nbsp;&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;&nbsp;|-file: f4.py

This package is called package and contain some sub packages and files. The sub package contain files too, and it can contain sub packages too. 

If the package is in the same directory, to import these packages you can do:
```
from Packages_A import f1   # This imports the f1 files from package A.
from Packages_A.Sub_package_A import f3   # This imports the f3 files from sub package A.
```

## Building packages 
Tutorial from Python [link](https://packaging.python.org/en/latest/tutorials/packaging-projects/).

Based on the official Python docs. There are some files which need to be configured. These are **setup.py** (most important file), **README.md**, **MANIFEST.in**.

### Using [MANIFEST.in](https://setuptools.pypa.io/en/latest/userguide/miscellaneous.html#using-manifest-in)

Needed when you need to package additional files that are not automatically included in a source distribution see. A MANIFEST.in file consists of commands, one per line, instructing setuptools to add or remove some set of files from the source distribution.



# Building a Pipeline using sklearn 
When using Sklearns pipeline, they must implement a fit and transform methods. While working, it is not always possible to ensure these are available. Therefore custom classes are made which just pass through the data.

e.g. code for custom fit_transform classes.

```
from sklearn.base import BaseEstimator, TransformMixin

class DemoTransformer(BaseEstimator, TransformMixin):
    def __init__(self):
        pass

    def fit(self, X, y=None):
        return self

    def transform(self, X):
        return X
```
