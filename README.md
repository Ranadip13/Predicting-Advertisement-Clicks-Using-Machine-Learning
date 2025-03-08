# Predicting Advertisement Clicks Using Machine Learning
The objective of this project is to predict whether a user will click on an advertisement on a website based on their behaviour and profile. When a user visits a site, businesses want to know if they are likely to engage with an ad. By analyzing past data on ad clicks and user activity, a model can be built to make better predictions. This helps businesses show ads to the right people and improve their marketing efforts.

In this project, a step-by-step approach to creating a Machine Learning predictive model for such scenarios was discussed. This flow can be used as a template to solve any supervised classification ML problem.
The flow of the case study is as below:
- Reading the data in python
- Defining the problem statement
- Identifying the Target variable
- Looking at the distribution of Target variable
- Basic Data exploration
- Visual Exploratory Data Analysis for data distribution (Histogram and Barcharts)
- Feature Selection based on data distribution
- Outlier treatment
- Missing Values treatment
- Visual correlation analysis
- Statistical correlation analysis (Feature Selection)
- Selecting final predictors for ML
- Converting data to numeric for ML
- Splitting the data into Training and Testing sample
- Standardization / Normalization of data (if required)
- Sampling and K-fold cross validation
- Trying multiple classification algorithms
- Selecting the best Model
- Deploying the best model in production

#### Data description: The business meaning of each column in the data is as below
- VistID: The id for the user visit on website
- Time_Spent: Average time spent by user on site in minutes
- Age: User age in years
- Area_Income: Average Income of geographical area of user
- Internet_Usage: Average minutes a day user spent on the internet
- Ad_Topic: Headline of the advertisement
- Country_Name: Country of user
- City_Code: City of user
- Male: Whether or not user was male
- Time_Period: Time at which consumer clicked on Ad
- Weekday: Name of the day
- Month: Name of the months
- Year: Which year the data is collected
- Clicked: 0 means not clicked and 1 means that user clicked the Ad.

Following the above steps, various classification machine learning algorithms were tried, including Logistic Regression, Decision Trees, Random Forest, AdaBoost, KNN, Support Vector Machines (SVM), and Naive Bayes, and their average accuracies were calculated. In this case, multiple algorithms produced similar average accuracy. Therefore, any one of them could be chosen. Adaboost is chosen as the final model due to its speed and effective use of predictors, as observed in its variable importance chart. It ensures that no single predictor dominates the decision, which is beneficial.

To deploy the model, the following steps are followed:
1.	Train the model using 100% of the available data.
2.	Save the model as a serialized file for storage and future use.
3.	Develop a Python function that integrates with front-end applications to take inputs and return predictions.
