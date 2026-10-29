# Data Science Notes: Data Analysis, SQL and EDA

Hands-on notebooks covering the foundations of the data science workflow: working with data in NumPy and pandas, querying SQLite from Python, and exploratory data analysis with feature engineering. Each notebook explains a topic and applies it to a real dataset.

> **Scope.** These are learning and reference notes, not a production project. The first three modules are complete; machine learning, deep learning and NLP modules are planned.

## Contents

### 01 · Data Analysis with Python

| Notebook | Topic |
| --- | --- |
| `01.1-Numpy` | Arrays, vectorised operations, universal functions, slicing, statistics and logical operations |
| `01.2-Pandas` | Series and DataFrames, accessing and manipulating data |
| `01.3-Data_Manipulation` | Missing values, renaming columns, data types, grouping and aggregation, merging and joining |
| `01.4-Reading_Data` | Reading data from different sources (CSV, Excel, remote files) |
| `01.5-Data_Visualization_with_Matplotlib` | Line, bar, histogram, scatter and pie charts; a sales data example |
| `01.6-Data_Visualization_with_Seaborn` | Line, bar, box, violin, histogram, KDE and pair plots; heatmaps |
| `01.7-Pandas_Exercise` | Exercises: indexing, cleaning, aggregation, merging, time series, MultiIndex, pivot tables |
| `01.8-Numpy_Excercise` | Exercises: array manipulation, broadcasting, linear algebra, fancy indexing |

### 02 · Working with SQLite3

| Notebook | Topic |
| --- | --- |
| `02.1-SQLite_and_Python` | Connecting to SQLite, creating tables, inserting and querying rows |
| `02.2-SQLite_Examples` | Worked examples: CRUD operations, advanced queries, transactions, relationships and backups |
| `Module_SQLite3_Assignments_Solution` | The same tasks with complete solutions |

### 03 · EDA and Feature Engineering

| Notebook | Topic |
| --- | --- |
| `03.1-Handling_Missing_Values` | Types of missing data, row and column deletion, mean, median and mode imputation |
| `03.2-Handling_Imbalanced_Dataset` | Oversampling, downsampling, SMOTE (`imbalanced-learn`) and outlier handling |
| `03.3-Data_Encoding` | One-hot, label, ordinal and target-guided ordinal encoding |
| `03.4-EDA_with_Red_Wine_Dataset` | Exploratory analysis and visualisation of red wine quality |
| `03.5-EDA_and_Feature_Engineering` | EDA and feature engineering on a flight price dataset, including one-hot encoding |
| `03.6-Data_Cleaning_and_EDA` | Cleaning, EDA and insights on Google Play Store app data |

## Running the Notebooks

Requirements: Python 3.9 or later and Jupyter.

```bash
pip install jupyter numpy pandas matplotlib seaborn scikit-learn imbalanced-learn openpyxl requests
jupyter lab
```

`sqlite3` is part of the Python standard library. The SQLite notebooks create their own example databases (`*.db`) when they run; these files are not tracked in Git.

## Data

**Included in the repository:**

| File | Source |
| --- | --- |
| `03-EDA_and_Feature_Engineering/data/winequality-red.csv` | [Wine Quality](https://archive.ics.uci.edu/dataset/186/wine+quality), UCI Machine Learning Repository (CC BY 4.0) |
| `01-Data_Analaysis_with_Python/data/data.csv`, `data.xlsx`, `sales_data.csv` | Small example files created for the reading and SQL exercises |

**Download before running the notebooks that use them:** third-party datasets are not redistributed here. Download them from Kaggle and save them under the given name:

| Save as | Download | Used by |
| --- | --- | --- |
| `03-EDA_and_Feature_Engineering/data/googleplaystore.csv` | `googleplaystore.csv` from [Google Play Store Apps](https://www.kaggle.com/datasets/lava18/google-play-store-apps) | `03.6-Data_Cleaning_and_EDA` |
| `03-EDA_and_Feature_Engineering/data/flight_price.xlsx` | `Data_Train.xlsx` from [Flight Fare Prediction MH](https://www.kaggle.com/datasets/nikhilmittal/flight-fare-prediction-mh) | `03.5-EDA_and_Feature_Engineering` |

**Generated when the notebooks run:** `01-Data_Analaysis_with_Python/data/wine.csv` (downloaded from the UCI [Wine](https://archive.ics.uci.edu/ml/machine-learning-databases/wine/) dataset by `01.4-Reading_Data`) and `03-EDA_and_Feature_Engineering/data/googleplaystore_cleaned.csv` (written by `03.6-Data_Cleaning_and_EDA`).

Check each source for its license terms before using the data outside of learning purposes.

## License

The code and notebooks are released under the [MIT License](LICENSE). The datasets are not covered by this license; they remain under the terms of their original sources listed above.
