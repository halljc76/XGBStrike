# XGBStrike
Repository for an application to the UNC Sports Analytics and Intelligence Laboratory (SAIL).

**Instructions for Running Code**
The notebook linked in this repsitory uses Python 3.10 and the following packages, each of which can be installed with the 'pip' command:
- pybaseball
- sklearn
- numpy
- pandas
- matplotlib
- seaborn
- xgboost
- hyperopt

Once installed, if cloning the repository, please run the following lines of Python code.
```{python}
cache.enable()
data = pd.DataFrame(statcast(start_dt = "2012-01-01", end_dt = "2022-12-23"))
data.to_csv("./pitch12to22.csv", index = False)
{python}

These lines will scrape and save (assuming the stability of the pybaseball package) data from the 2012-2022 MLB seasons. 
If you wish, you may change the dates to obtain different data and observe the model performance, as well as altering the predictors used.
