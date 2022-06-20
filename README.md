# Disaster Response Pipeline Project

## File Description:
      1. process_data.py: This python excutuble code takes as its input csv files containing message data and
         message categories (labels), and then creates a SQL database
      2. train_classifier.py: This code trains the ML model with the SQL data base
      3. ETL Pipeline Preparation.ipynb: process_data.py development procces
      4. ML Pipeline Preparation.ipynb: train_classifier.py. development procces
      5. data: This folder contains sample messages and categories datasets in csv format.
      6. app: cointains the run.py to iniate the web app.


### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/MLclassifier.pkl`

2. Go to `app` directory: `cd app`

3. Run your web app: `python run.py`

4. Click the `PREVIEW` button to open the homepage
