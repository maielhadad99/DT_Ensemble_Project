# DT_Ensemble_Project

Project on Bagging and Boosting ensemble model:

The data contains observations of about 240 million clicks, and whether a given click resulted in a download or not (1/0):

The detailed data dictionary is mentioned here:

ip: ip address of click.

app: app id for marketing.

device: device type id of user mobile phone (e.g., iphone 6 plus, iphone 7, huawei mate 7, etc.)

os: os version id of user mobile phone

channel: channel id of mobile ad publisher

click_time: timestamp of click (UTC)

attributed_time: if user download the app for after clicking an ad, this is the time of the app download

is_attributed: the target that is to be predicted, indicating the app was downloaded

Let's try finding some useful trends in the data.

**1. Explore the dataset for anomalies and missing values and take corrective actions if necessary.**

**2. Which column has maximum number of unique values present among all the available columns**

**3. Use an appropriate technique to get rid of all the apps that are very rare (say which comprise of less                than 20% clicks) and plot the rest..** 

**4. By using Pandas derive new features such as - 'day_of_week' , 'day_of_year' , 'month' , and 'hour' as                  float/int datatypes using the 'click_time' column . Add the newly derived columns in original dataset.**

**5. Divide the data into training and testing subsets into 80:20 ratio(Train_data = 80% , Testing_data = 20%) and
     check the average download rates('is_attributed') for train and test data, scores should be comparable.**

**6. Apply XGBoostClassifier with default parameters on training data and make first 10 prediction for Test data.          NOTE: Use y_pred = model.predict_proba(X_test) since we need probabilities to compute AUC.** 

**7. On evaluating the predictions made by the model what is the AUC/ROC score with default hyperparameters.**
