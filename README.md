# customer_churn_prediction
A case study to predict customer churn for a ride sharing company

A ride-sharing company (Company X) is interested in predicting rider retention.
To help explore this question, they provided a sample dataset of a group of
users who signed up for an account in January 2014. The data was pulled on July
1, 2014; we consider a user retained if they were “active” (i.e. took a trip)
in the preceding 30 days (from the day the data was pulled). In other words, a
user is "active" if they have taken a trip since June 1, 2014. The data,
`churn.csv`, is in the [data](data) folder.  The data are split into train and
test set.

The problem to be solved here is **what factors are
the best predictors for retention**, and by doing data analysis to offer
suggestions to operationalize those insights to help Company X.
Therefore the task is not only to build a model that minimizes error,
but also a model that allows you to interpret the factors that
contributed to your predictions.

Here is a detailed description of the data:

- `city`: city this user signed up in phone: primary device for this user
- `signup_date`: date of account registration; in the form `YYYYMMDD`
- `last_trip_date`: the last time this user completed a trip; in the form `YYYYMMDD`
- `avg_dist`: the average distance (in miles) per trip taken in the first 30 days after signup
- `avg_rating_by_driver`: the rider’s average rating over all of their trips
- `avg_rating_of_driver`: the rider’s average rating of their drivers over all of their trips
- `surge_pct`: the percent of trips taken with surge multiplier > 1
- `avg_surge`: The average surge multiplier over all of this user’s trips
- `trips_in_first_30_days`: the number of trips this user took in the first 30 days after signing up
- `luxury_car_user`: TRUE if the user took a luxury car in their first 30 days; FALSE otherwise
- `weekday_pct`: the percent of the user’s trips occurring during a weekday


## Work Flow

1. Performed any cleaning, exploratory analysis, and/or visualizations to use the
provided data for this analysis.

2. Built a predictive model to help determine the probability that a rider will
be retained.

3. Evaluated the model.  Focus on metrics that are important for your *statistical
model*.

4. Identified / interpreted features that are the most influential in affecting
my predictions.

5. Performed validation on model. Issues such as
leakage.  References on leakage: [this essay on
Kaggle](https://www.kaggle.com/wiki/Leakage), and [Leakage in Data
Mining: Formulation, Detection, and Avoidance](https://www.cs.umb.edu/~ding/history/470_670_fall_2011/papers/cs670_Tran_PreferredPaper_LeakingInDataMining.pdf).

6. Repeated 2 - 5 until finding a satisfactory model.
