# cap5768-introduction-to-data-science

CAP5768 Introduction to Data Science Fall 2019

Credits:

* [Professor Dr. Oge Marques](https://www.ogemarques.com/)
* Our textbooks: [Python Data Science Handbook](https://colab.research.google.com/github/jakevdp/PythonDataScienceHandbook/blob/master/notebooks/Index.ipynb#scrollTo=sr_2etKoQWhh), and [Think Stats 2](https://greenteapress.com/thinkstats2/thinkstats2.pdf)
* DataCamp courses: [Statistical Thinking in Python part 1](https://www.datacamp.com/courses/statistical-thinking-in-python-part-1) and [part 2](https://www.datacamp.com/courses/statistical-thinking-in-python-part-2)

Quick "get started" guide:

1. Clone this repository
1. `cd` to the repository's directory
1. Optional: create a [Python virtual environment](https://docs.python.org/3/tutorial/venv.html)
    1. `python3 -m venv env`
    1. `source env/bin/activate` (Windows: `env\Scripts\activate.bat`)
    1. `python -m pip install --upgrade pip`
1. `pip install -r requirements.txt`
1. `jupyter lab`
1. Navigate to the assignments and open the notebook

Other data science resources similar to this one:

* [IEEE ICMLA 2019 data science tutorial](https://github.com/fau-masters-collected-works-cgarbin/ieee-icmla-2019-data-science-tutorial): a structured introduction to data science, with smaller notebooks, each for a specific topic.
* [How to write well-structured, understandable, reliable, flexible Jupyter notebooks](https://github.com/fau-masters-collected-works-cgarbin/writing-good-jupyter-notebooks).

## Assignment 1

[Assignment 1](./assignment1) is a warm-up exercise to get used to NumPy and Pandas in a Jupyter environment.

Covered in this assignment:

* Get a Jupyter Lab environment up and running (see [this wiki page](https://github.com/fau-masters-collected-works-cgarbin/cap5768-introduction-to-data-science/wiki/Minimalist-JupyterLab-setup-with-a-handful-of-extensions))
* Learn and apply NumPy and Pandas (see notes [in this wiki page](https://github.com/fau-masters-collected-works-cgarbin/cap5768-introduction-to-data-science/wiki/Notes-from-Python-Data-Science-Handbook))
* Read data from .csv files
* Uses Pandas `DataFrame` and `Series` filter and aggregation functions
* Find correlations analytically with Pearson correlation coefficient and aggregated statistics
* Find correlations with graphs (Seaborn `regplot`)
* Formulate and verify hypotheses with analytical (e.g. aggregation by type) and graphical support (e.g. box plots)

## Assignment 2

[Assignment 2](./assignment2) is about exploration of datasets (manipulate, summarize, visualize).

Covered in this assignment:

* Combine multiple datasets into one, using common fields across the datasets
* Summarize, filter and sort data with `pivot_table`, `groupby`, `query`, `eval` and other functions
* Visualize datasets with Matplotlib and `DataFrame.plot`
* More formulation and verification of hypotheses with analytical (e.g. aggregation by type) and graphical support

## Assignment 3

[Assignment 3](./assignment3) is when we switched from analytics to statistics, the first chapters of [Think Stats 2](https://greenteapress.com/wp/think-stats-2e/).

Covered in this assignment:

* Selecting the number of bins for histograms ("binning bias")
* Beyond histograms: swarm plots and box plots
* Cumulative distribution function (CDF)
* Correlation with Pearson and Spearman functions

## Assignment 4

[Assignment 4](./assignment4) explores modeling: how to identify the type of a distribution and its parameters, validate the distribution against a theoretical model, then use the model to answer questions about the distribution. [Part 1 of DataCamp's Statistical Thinking in Python](https://www.datacamp.com/courses/statistical-thinking-in-python-part-1) was a helpful resource.

Covered in this assignment:

* PDF and CDF of exponential distributions
* Find the type and parameters of an empirical distribution
* Use the parameters to simulate the distribution and answer questions about it
* Calculate moments and skewness

## Assignment 5

[Assignment 5](./assignment5) covers hypotheses testing with simulations and p-value calculation. Cassie Kozyrkov's [Statistics for people in a hurry](https://towardsdatascience.com/statistics-for-people-in-a-hurry-a9613c0ed0b) was very helpful in understanding the concepts of what we are attempting here, especially the meaning of the null hypothesis.

Covered in this assignment:

* Permutate the empirical data to run experiments (using `numpy.random.permutation()`)
* Decide what pieces of the dataset we need to permutate (all of them, only one?)
* Calculate the p-value from the experiments
* Interpret the p-value

## Assignment 6

[Assignment 6](./assignment6) covers regression analysis: how to add polynomial features, then perform linear regression on the enhanced dataset, evaluate results with R<sup>2</sup> score and regularize with Ridge and Lasso.

Covered in this assignment:

* Perform linear regression with Numpy `polyfit()`
* Add features to improve fitting with `PolynomialFeatures()`
* Perform Linear regression with scikit-learn `LinearRegression()`
* Perform all steps together with a pipeline
* Regularize with Ridge and Lasso to prevent overfitting
* Use `RidgeCV()` and `LassoCV()` for hyperparameter search
* Evaluate the linear regression results with the R<sup>2</sup> score
* Choose an optimal polynomial degree by comparing R<sup>2</sup> score
* To not trust only the summary statistics (Anscombe's quartet)

## Final project

In the [final project](./final-project) we review concepts we learned early in the course,
and use the techniques we learned later.

Covered in the final project:

* DataFrame `describe()`, to view summary statistics at a glance. All the important values are available with one function call.
* How much we get out-of-the-box from the [`pandas_profiling`](https://github.com/pandas-profiling/pandas-profiling) package. It is like a "mini EDA" with one line of code.
* The `verbose` parameter to follow the progress of long-running scikit-learn tasks.
* Pay attention to random_state in the scikit-learn APIs to get consistent results.
* Use `GridSearchCV()` to find parameters for a classifier.
* The power and simplicity of Naive Bayes classifiers, even for seemly complex tasks such as digit classification. It can be used as a baseline before attempting more
  complex solutions.
* The power and simplicity of Naive Bayes classifiers, even for seemly complex tasks such as digit classification. It can be used as a baseline before attempting more complex solutions.
* How to use seaborn's `heatmap` for confusion matrix visualization. More specifically, the trick to zero out the diagonal with NumPy fill_diagonal() to make the mistakes stand out in the graph.
* The power and simplicity of Naive Bayes classifiers, even for seemly complex tasks such as digit classification. It can be used as a baseline before attempting more complex solutions.
* How surprisingly good random forest classifiers perform, achieving 97% in the digit classification without much work. Another case of "try this before pulling your neural network card" case. Random forests may have an edge, especially with the emphasis on explainable AI, because even laypeople can understand them.
* The small number of components we need to explain variability (the PCA section).
* Finally getting a chance to play with [OpenCV](https://opencv.org/) and see first-hand how easy and feature-rich it is.
