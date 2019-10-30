# cap5768-introduction-to-data-science
CAP5768 Introduction to Data Science Fall 2019

## Assignment 1

[Assignment 1](./assignment1) is a warm-up exercise, to get used to NumPy and Pandas in a Jupyter environment.

Covered in this assignment:

* Get a Jupyter Lab environment up and running (see [this wiki page](https://github.com/fau-masters-collected-works-cgarbin/cap5768-introduction-to-data-science/wiki/Minimalist-JupyterLab-setup-with-a-handful-of-extensions))
* Learn and apply NumPy and Pandas (see notes [in this wiki page](https://github.com/fau-masters-collected-works-cgarbin/cap5768-introduction-to-data-science/wiki/Notes-from-Python-Data-Science-Handbook))
* Read data from .csv files
* Uses Pandas `DataFrame` and `Series` filter and aggregration functions
* Find correlations analytically with Pearson correlation coefficient and aggregated statistics
* Find correlations with graphs (Seaborn `regplot`)
* Formulate and verify hypotheses with analytical (e.g. aggregation by type) and graphical support (e.g. box plots)

## Assignment 2

[Assignment 2](./assignment2) is about exploration of datasets (manipulate, summarize, visualize).

Covered in this assignment:

* Combine multiple datasets into, using common fields across the datasets
* Summarize, filter and sort data with `pivot_table`, `groupby`, `query`, `eval` and other functions
* Visualize datasets with Matplotlib and `DataFrame.plot`
* More formulation and verification of hypotheses with analytical (e.g. aggregation by type) and graphical support

## Assignment 3

[Assignment 3](./assignment3) is when we switched from analytics to statistics, the first chapters of [Think Stats 2](https://greenteapress.com/wp/think-stats-2e/).

Covered in this assignment:

* Selecting number of bins for histograms ("binning bias")
* Beyond histograms: swarm plots and box plots
* Cumulative distribution function (CDF)
* Correlation with Pearson and Spearman functions

## Assignment 4

[Assignment 4](./assignment4) explores modeling: how to identify the type of a distribution and its parameters, validate the dsitrubtion against a theoretical model, then use the model to answer questions about the distribution. [Part 1 of DataCamp's Statistical Thinking in Python](https://www.datacamp.com/courses/statistical-thinking-in-python-part-1) was a useful resource.

Covered in this assignment:

* PDF and CDF of exponential distributions
* Find the type and parameters of an empirical distribution
* Use the parameters to simulate the distribution and answer qeustions about it
* Calculate moments and skewness

