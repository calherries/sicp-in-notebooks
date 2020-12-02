SICP
====

## Read SICP in Jupyter Notebooks with MIT Scheme, without any setup

> "If SICP were written in 2020, it would be in a Jupyter Notebook" - me yesterday

If you want to read SICP from a Jupyter Notebook, you now have two options to get started:
- Option 1: Run SICP straight from the browser
- Option 1: Build and run SICP from a docker container

Option 1: Run straight from the browser
------------------------------------

[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/callum-herries/sicp-notebooks/master?filepath=0.0_Structure_and_Interpretation_of_Computer_Programs.ipynb)

Follow this link to create your own binder:
[https://mybinder.org/v2/gh/callum-herries/sicp-notebooks/master](https://mybinder.org/v2/gh/callum-herries/sicp-notebooks/master)

Clicking this link will create a docker container for you with a ready-to-use MIT Scheme Jupyter kernel. Any changes you make to the notebooks will persist when you close the browser, as long as you use the same URL.

Option 2: Build and run a docker container
----------------------------------------

Clone this repo and build the container from scratch.

On Linux/Mac:

```
git clone git@github.com:callum-herries/sicp-notebooks.git
cd sicp-notebooks
docker build -t sicp-notebooks .
docker run -it --rm -p 8888:8888 -v ${PWD}:/home/jovyan sicp-notebooks
```

License
-------

The content of the notebooks, and diagrams in fig directory are licensed under Creative Commons Attribution-ShareAlike 4.0 International License (cc by-sa).
