# Customer Behaviour on Starbucks rewards Mobile app
 
![image](https://user-images.githubusercontent.com/58060845/144759810-e3151b07-cbf4-44b9-8309-195cb281fddb.png)

***This Project is based on Predictive Analysis.***

In this project, we would go through the predictive modeling technique for customer behavior through Starbucks dataset example. Starbucks provided simulated data that mimics customer behavior on the Starbucks rewards mobile app. Once every few days, Starbucks sends out an offer to users of the mobile app. An offer can be merely an advertisement for a drink or an actual offer such as a discount or BOGO (buy one get one free). Some users might not receive any offer during certain weeks. Not all users receive the same offer, and this data set is a simplified version of the real Starbucks app because the underlying simulator only has one product whereas Starbucks actually sells dozens of products.
Starbucks wants to connect offer data, customer data and transaction data (operational data) to gain insights about customer behavior and overall effectiveness of offers as a value for business.
With the above key statement in mind, below is the main objective or problem motivation or problem statement:

_**Build a model that predicts whether a customer would respond to an offer or not.**_

![image](https://user-images.githubusercontent.com/58060845/144759824-af44f993-f19a-4663-baf5-75333b377996.png)
# Project Approach
The entire analysis would contain below steps:
 1)Analyse each of the portfolio, profile and transaction data.
 2)Clean and transform each of the portfolio, profile and transaction data.
 3)Combine portfolio, profile and transaction data.
 4)Select a performance metric to analyse performance of the model and to compare different models.
 5)Compute the performance of a baseline model against which performance of other different models would be compared.
 6)Select best performing model based on the metric and training time.
 7)Calculate the feature importances given by best estimator of the trained model.
 8)Compute the performance of best model on test set and visualize the performance via confusion matrix plot.

![image](https://user-images.githubusercontent.com/58060845/144759901-5d22b453-08be-492a-aa56-09305f0c7681.png)

# Datasets

The data is contained in three files:

* portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
* profile.json - demographic data for each customer
* transcript.json - records for transactions, offers received, offers viewed, and offers completed

_Here is the schema and explanation of each variable in the files:_

1)portfolio.json
* id (string) - offer id
* offer_type (string) - type of offer ie BOGO, discount, informational
* difficulty (int) - minimum required spend to complete an offer
* reward (int) - reward given for completing an offer
* duration (int) - time for offer to be open, in days
* channels (list of strings)

2)profile.json
* age (int) - age of the customer
* became_member_on (int) - date when customer created an app account
* gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
* id (str) - customer id
* income (float) - customer's income

3)transcript.json
* event (str) - record description (ie transaction, offer received, offer viewed, etc.)
* person (str) - customer id
* time (int) - time in hours since start of test. The data begins at time t=0
* value - (dict of strings) - either an offer id or transaction amount depending on the record

![image](https://user-images.githubusercontent.com/58060845/144759850-1eff3e0a-5ae3-4e7c-8470-d6ef206da721.png)

Have a nice coffee yáll :)

