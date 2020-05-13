# Disaster Response Pipeline Project
This project is a part of the Data Science Nanodegree Program by Udacity.

### Table of Contents
1. [Introduction](#introduction)
2. [File Descriptions](#filedescriptions)
3. [Instructions](#instructions)
4. [Results](#results)
5. [Acknowledgements](#acknowledgmements)

### 1. Introduction <a name="introduction"></a> 
The aim of this project is to build a machine learning model to analyze disaster data from [Figure Eight](https://www.figure-eight.com/) that classifies disaster messages, and show the result in an interactive webpage.

### 2. File Descriptions <a name="filedescriptions"></a>
- app
| - template
| |- master.html  # main page of web app
| |- go.html  # classification result page of web app
|- run.py  # Flask file that runs app

- data
|- disaster_categories.csv  # data to process 
|- disaster_messages.csv  # data to process
|- process_data.py  # script to process data
|- DiastersDB.db   # database to save clean data to

- models
|- train_classifier.py   # script to train model
|- classifier.pkl  # saved model 

- results
|- screenshot-1    # distribution of message categories
|- screenshot-2    # top 10 distribution of message categories in percentage
|- screenshot-3    # distribution of message genres
|- screenshot-4    # an example of disaster response webpage

- README.md

### 3. Instructions <a name="instructions"></a>
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisastersDB.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisastersDB.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/

### 4. Results <a name="results"></a>
![screenshot-1](https://view6914b2f4.udacity-student-workspaces.com/files/home/workspace/results/screenshot-1.png)

![screenshot-2](https://view6914b2f4.udacity-student-workspaces.com/files/home/workspace/results/screenshot-2.png)

![screenshot-3](https://view6914b2f4.udacity-student-workspaces.com/files/home/workspace/results/screenshot-3.png)

![screenshot-4](https://view6914b2f4.udacity-student-workspaces.com/files/home/workspace/results/screenshot-4.png)

### 5. Acknowledgmements <a name="acknowledgmements"></a>
I would like to thank [Udacity](https://www.udacity.com/) and [Figure Eight](https://www.figure-eight.com) for their support in this project.
