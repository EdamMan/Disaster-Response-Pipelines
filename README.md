Disaster Response Pipelines

Required libraries

- Machine Learning Libraries: NumPy, SciPy, Pandas, Sciki-Learn
- Natural Language Process Libraries: NLTK
- Python
- SQLlite Database Libraqries: SQLalchemy
- Web App and Data Visualization: Flask, Plotly

Motivation

In this project i have analyzed disaster responses data given by udacity to build a model for an API that classifies disaster messages.

Executing Program:

1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        'python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/InsertDatabaseName.db'
    - To run ML pipeline that trains classifier and saves
        'python models/train_classifier.py data/InsertDatabaseName.db models/new_model.pkl'
    - Run the following command in the app's directory to run your web app.
     	 python run.py
    - Go to http://0.0.0.0:3001/


File

- ETL Pipeline Preparation.ipynb: process_data.py
- ML Pipeline Preparation.ipynb: train_classifier.py
- process_data.py: A data cleaning pipeline that:
  - Loads the messages
  - Merges the two datasets
  - Stores it in a SQLite database

- train_classifier.py: A machine learning pipeline that:
  - Loads data from the SQLite database
  - Splits the dataset into training and test sets
  - Builds a text processing and machine learning pipeline
  - Outputs results on the test set

Github link : https://github.com/EdamMan/Disaster-Response-Pipelines