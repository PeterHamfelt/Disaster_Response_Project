# Disaster_Response_Project

## 1. Project Overview
#### Purpose of the project to build a web app to aid emergency workers which can help to classify disaster response messages in various categories and the emergency worker can send the messages to the appropriate disaster relief agency to take proper action. The app will also display visualizations of the data.

## 2. Pre-requisites
#### Python (>= 3.6.3)
#### Pandas (>= 0.23.3)
#### NLTK (>= 3.2.5)
#### Scikit-learn (>= 0.19.1)
#### SQLAlchemy (>= 1.2.19)
#### Flask framework (>= 0.12.5)
#### Plotly (>= 2.9.0)
#### Bootstrap (>= 3.3.7)

## 3. Project Implementation 
### This project has below three parts. 
#### 3.1 ETL Development - This part has below steps: 
#### - Import libraries and load datasets.
#### - Merge datasets
#### - Split categories into separate category columns
#### - Convert category values to just numbers 0 or 1.
#### - Replace categories column in df with new category columns.
#### - Remove duplicates.
#### - Save the clean dataset into an sqlite database

### 3.2 ML Pipeline Development
#### - Load data from database.
#### - Tokenize the text data
#### - Build a machine learning pipeline
#### - Train the model pipeline
#### - Evaluate the model
#### - Export the model as a pickle file

### 3.3 Web App Development
#### - Buikd an interface to enter new message and classify it by selecting the related categories from a list below
#### - Provide vizualizations related to the database

## 4. How to run
### 4.1 ETL Pipeline - python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db
### 4.2 ML Pipeline - python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl
### 4.3 Web App - a. Go to `app` directory: `cd app`, b. Run the web app: `python run.py`, c. Click the `PREVIEW` button to open the homepage 

## 5. Repository Structure
### 5.1 app folder contains run.py and template folder which has master.html and go.html
### 5.2 data folder contains disaster_message.csv, disaster_categories.csv files and process_data.py (ETL Pipeline) and DisasterResponse.db
### 5.3 models folder contains train_classifier.py (ML pipeline) and classifier.pkl (saved model)

## 6. Acknowledgements
### 6.1 Dataset Credit: Udacity
### 6.2 Others: Thanks to Udacity for excellent course material and also to the mentors for timely help.
