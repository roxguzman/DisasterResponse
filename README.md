# Disaster Response Pipeline Project

### Instructions:
To run the scripts you need to have the following:
1. Create 3 directories, with the names app, data and models.
2. The directory app, needs to have the run.py and a directory called templates, in the templates directory you need to have the go.html       and master.html.
3. The data direcory requires to have disaster_category.csv, disaster_messages.csv and process_data.py
4. The models directory requires the script classifier.pkl and train_classifier.py. I can't copy here the classifier.pkl because the size is bigger than what this repository accepts.
5. After the you complete all of this then run the following commands in the project's root directory to set up your database and model.
    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/disaster_response.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/disaster_response.db models/classifier.pkl`
6. Run the following command in the app's directory to run your web app.
    `python run.py`
7. Open another terminal and type env| grep WORK, this will give you the SPACEID and SPACEDOMAIN, replace those values and type the below. 
8. Then go to https://SPACEID-3001.SPACEDOMAIN
