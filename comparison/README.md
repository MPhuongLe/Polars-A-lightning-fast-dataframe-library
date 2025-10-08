# Experiment: A Comparison between Pandas and Polars

### Experiment
We generate a dataset of 21 files of 3 types and 7 sizes:
- Types: numerical columns only, object columns only (aka. string) and mixed (some are numerical, some are object).
- Sizes: 100 000, 200 000, 500 000, 1 000 000, 2 000 000, 5 000 000, 10 000 000 (rows)

We do experiment on the following operations: read csv file, aggregation (min, max, mean, median), query (filter, filter + select), sort, group by (on string column, on category type column), join, compound manipulation (here we observe Polars lazyframe as well). 

The observed target of this experiment is the `run time` each of the two libraries needs to operate on the given files. 

You can get the experiment results right in this directory (`csv` files). However, if you want to know how was the experiment carried out in detail, visit [Kaggle](https://www.kaggle.com/datasets/vhonghoavin/ida2024-polars-vs-pandas-data/data).

The experiment is divided into four notebooks, each comparing the performance of `Pandas` and `Polars` in different aspects:
- [Notebook 01](https://www.kaggle.com/code/vhonghoavin/experiment-01-read-aggregation-query): Focus on file reading, some aggregation opperators and some simple queries.
- [Notebook 02](https://www.kaggle.com/code/vhonghoavin/experiment-02-group-by-sort): The performance in groupby and sort opperators.
- [Notebook 03](https://www.kaggle.com/code/vhonghoavin/experiment-03-join) : The performance in join opperator.
- [Notebook 04](https://www.kaggle.com/code/caokhoihuynh/experiment-04-manipulation) : The performance in data manipulation.

### Visualization

We visualize the experiment results in the notebook `TomatoGroup-Polars-Comparison.ipynb`. The outputted graphs are also included in our slides (in the `./slide` directory).
