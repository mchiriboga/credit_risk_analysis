# Credit Risk Analysis

## Dependencies

The analysis was developed using Python 3.7.3 with [Jupyter Notebook](https://jupyter.org) 5.7.8.


 Additionaly, the following packages and versions were used:
- [ipywidgets](https://ipywidgets.readthedocs.io/en/stable/user_install.html) 7.5.0
- [numpy](https://numpy.org) 1.16.4
- [pandas](https://pandas.pydata.org) 0.24.2
- [pandas-profiling](https://github.com/pandas-profiling/pandas-profiling) 2.4.0
- [sklearn](https://scikit-learn.org/stable/) 0.22.1
- [XGBoost](https://xgboost.readthedocs.io/en/latest/index.html) 0.90

## Instructions

To run the notebook, enter `jupyter notebook` into the terminal and navigate to the folder containing the `credit_risk_analysis.ipynb` file. The `train_dataset.csv` and `test_dataset.csv` must be placed within a `data` folder, in the same directory as the notebook file.

## Expected Performance

The final model trained achieved a score of 0.7766 with the Area Under the ROC curve metric, against the validation set, which was split from `train_dataset.csv`. This data was not used for model tuning or training, and is thus the best estimate for the expected performance of the model predictions against the test data in `test_dataset.csv`.

The predictions are saved to `predictions.csv`, as required.

## Using the Model's Predictions to Make Credit Decisions

The probability of default can be used to help a lender determine the risk of a loan. A high probability of default may warn the lender so that they may change the terms of the loan accordingly, for example raising interest rates for higher risk loan, or even denying the loan altogether. Conversely, lower risk clients can receive better terms on their loans.
