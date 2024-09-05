# Hotel-Booking-Cancellation-Prediction
Developed a predictive model to forecast hotel booking cancellations by analyzing customer and  booking data. 
Identified key patterns to enhance booking strategies and improve operational  efficiency. 
By analyzing historical booking data, the model aims to identify patterns and factors that contribute to cancellations.

# Dataset Link - https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand

# Assumptions
• Sufficient Historical Data: The historical booking data is assumed to be representative enough to generalize patterns to future bookings.

• Independent Observations: The observations which are made are independent of each other.

• Customer Behavior Stability: Customer behavior patterns are assumed to remain consistent over time, allowing past data to inform future predictions.

• Removal of Personally Identifying Data: All personally identifying information have been removed from the data.

• We have assumed that there are many overlapping values between the features distribution_channel and market_segment from the heatmap that we have plotted and so we have dropped the distribution_channel column.

• We have assumed that reservation_status and reservation_status_date columns are cases of data leakage as they are highly correlated with the target variable(is-cancelled) with a value of -0.91.

• We have assumed that the unimportant features can induce complexity in the model and also lead to lower model performance, so we have dropped these columns.

# Design Decisions
• Data ingestion: Fetching data from Amazon S3 bucket.

• Libraries Used: Pandas, numpy, matplotlib, scikit-learn, seaborn.

• Exploratory Data Analysis: Sweet Viz Profiling, Y-data Profiling, Correlation of features with the Target variable, Pair-plot , Analysis of the features.

• Data Preprocessing: Separating numerical and categorical features, Encoding Categorical features- Label Encoder, Handling of missing values, Feature Selection.

• Model Selection: Logistic Regression, Random Forest, XGBoost Classifier, Neural Networks(ANN).

• Deployment: AWS Sagemaker - It is a fully managed service that provides tools to build,train and deploy ML models at a scale. It simplifies the process of developing ML models by handling infrastructure, making it easier to focus on model deployment.


