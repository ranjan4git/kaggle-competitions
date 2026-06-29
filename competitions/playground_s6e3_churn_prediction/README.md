[Link to the kaggle competition](https://www.kaggle.com/competitions/playground-series-s6e3/)


Steps:

1. Inside the terminal, go to the competitions folder, `cd <directory_path>`

2. Download the dataset, 
`kaggle competitions download -c playground-series-s6e3`

This will download a zip file in the directory.

3. Unzip the data in the data directory <br>
For Windows PowerShell:
`Expand-Archive playground-series-s6e3.zip data` 
<br>
For Bash:
`unzip playground-series-s6e3.zip -d data`

4. Create a virtual environment,
`python -m venv venv`
Activate:
`venv\Scripts\activate`

5. *Since this is the first competition* Install basic modules,
`pip install pandas, numpy, scikit-learn, lightgbm,xgboost, catboost, optuna, jupyter`
Now save 
`pip freeze > requirements.txt`

At this point, you should do your first commit of the competition, right?

6. Submission
`kaggle competitions submit -c playground-series-s6e3 -f outputs/baseline_rf_num_only_submission.csv  -m "Baseline RF numeric"`