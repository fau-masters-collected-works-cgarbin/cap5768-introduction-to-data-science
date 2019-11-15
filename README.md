# cap5768-introduction-to-data-science

CAP5768 Introduction to Data Science Fall 2019

Credits:

* Professor Dr. Oge Marques
* Our textbooks: [Python Data Science Handbook](https://colab.research.google.com/github/jakevdp/PythonDataScienceHandbook/blob/master/notebooks/Index.ipynb#scrollTo=sr_2etKoQWhh), and [Think Stats 2](https://greenteapress.com/thinkstats2/thinkstats2.pdf)
* DataCamp courses: [Statistical Thinking in Python part 1](https://www.datacamp.com/courses/statistical-thinking-in-python-part-1) and [part 2](https://www.datacamp.com/courses/statistical-thinking-in-python-part-2)

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

## Assignment 5

[Assignment 5](./assignment5) covers hypotheses testing with simulations and p-value calculation. Cassie Kozyrkov's [Statistics for people in a hurry](https://towardsdatascience.com/statistics-for-people-in-a-hurry-a9613c0ed0b) was very helpful to understand the concepts of what we are attempting here, especially the meaning of the null hypothesis.

Covered in this assignment:

* Permutate the empirical data to run experiments (using `numpy.random.permutation()`)
* Decide what pieces of the dataset we need to permutate (all of them, only one of them?)
* Calculate the p-value from the experiments
* Interpret the p-value
