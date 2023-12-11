### Business Problem Statement:
As the Traditional banking system relies heavily on the credit history of one individual, many people such as students or unemployed fail to establish their credit scores. Taking advantage of their financial vulnerability, these groups of people are targeted by untrustworthy lenders. Home Credit is on mission to change this paradigm by positively targeting these unbanked population to help them in safe and secure borrowing experience. Home Credit leverages telco and transactional data to assess an individual's repayment capabilities. They need some extra help in identifying which clients are most likely to fail on their loans/ which clients are capable of repaying back to maintain its financial stability, improve lending decisions and prevent losses. Our team moto is to help them in unlocking the full potential that data could serve to help them in making informed lending decisions.
Our objective is to increase the precision of loan repayment estimates by utilizing exploratory data analysis (EDA) and statistical methods to acquire deep insights into Home Credit's loan application data. Through rigorous data investigation, we try to find patterns, trends, and potential risk factors within the dataset. Our main goal is to enable Home Credit to make data-driven lending decisions that lower the risk of default without denying credit to qualified customers. The improved accuracy of loan repayment predictions, which will support Home Credit's financial stability and customer happiness, will serve as a barometer for the project's performance.

### Groups Solution:
Our solution to this problem would include the development of supervised predictive classification models since we have historical labelled data and as the outcome of the target variable is binary with values of 0 and 1, where 0 indicating timely loan repayment and 1 signifying potential repayment difficulties. We employed sophisticated techniques such as Logistic Regression and use of ensemble methods for extracting a list of customers with higher probabilities of loan repayment. The client’s repayment prediction will be based on alternate data to loan history such as telco and transactional information.
As a part of EDA, we have undertaken the following steps:
1.	Import & inspect dataset along with the target variable.
2.	Explore the relationship between target and predictors.
3.	Scope of missing values; imputing 
4.	One hot encoding of the categorical variables
5.	Univariate analysis
6.	Bivariate analysis
7.	Testing for Hypothesis
8.	Joining the Bureau and previous application tables and inspecting again
9.	Did feature engineering and created new features to be valuable to credit risk domain which have helped improve model AUC.
As a part of Pre-Modelling, we have used the following techniques:
1.	Split the train and test data in the ratio of 80-20
2.	Since the logistic regression is sensitive to unscaled data, we have scaled the data such the all the features fall under the range of 0-1
3.	We used k-fold cross-validation (Grid Search) with 5 folds to prevent over-fitting.
4.	To deal with class imbalance,
•	Under (Down sampling): Down sampled the majority class to match it with the number of instances of minority class.
•	Smote Sampling: We over sampled the minority class by creating synthetic data.
For modeling, we have used this cleaned data set to predict the loan default on different machine learning methods such as Logistic Regression, Random Forest, Neural Net, XGBoost and Light GBM. For better model performance we did hyperparameter tuning and to handle class imbalance in our data we employed sampling techniques as explained above. We evaluated these models’ using metrics like ROC-AUC and accuracy scores along with their Kaggle scores. The final model is chosen based on the highest Kaggle score. We obtained superior performance with Light BGM with a test accuracy of 0.83, Train and test ROC-AUC of 0.84 and 0.77 showing its balanced performance with a Kaggle score of 0.76.

### Problems Encountered in the project:
•	One of the major concerns was while running Neural Net, we encountered resource intense issues, we ran out of RAM and hence needed to discard Neural Net for further processing.
•	As there is a class imbalance in our dataset, we opted sampling techniques such as Down Sampling and Smote Sampling which were additional steps for modeling to help us finalize the final model.
•	We observed that the modelling scores were low or not as expected, so we tried to change the parameters, tried a few combinations to get more optimal performance scores.

### Important Features:
 

 
Ext_Source_3, Ext_Source_2 are the most important features in our data from Shap analysis and by feature Engineering. These helps in home credit to know on which factors to focus on.

### My contribution to the project:
Firstly, I did data cleaning by finding the missing values and removed the columns with missing values with a threshold more than 45% except EXT_Source_1 and removed highly correlated features with a threshold of 0.75 and low correlated features with a threshold of 0.04. Then I imputed the missing values with mean and mode and did one-hot encoding to deal with categorical columns.
As a group team member, I did Feature Engineering Research & Implementation, Feature Scaling & normalization for Logistic Regression, Split the train and test data in the ratio of 80-20. Employed Logistic Regression and Light GBM Model, Tuned Light GBM model. I analyzed the results of all the models including mine and other team members. I summarized and interpreted the results from a business perspective. Did the final Edits and formatting of the notebook and collaborated with the team in preparing and presenting the PowerPoint presentation.

### Business Value/ Recommendations:

•	We can predict model decisions using Tree Explainer.
•	These model predictions help home credit in Improved decision making with low risk.
•	Automated, faster, efficient & streamlined loan approval process. 
•	Helps them in tailoring credit limits, interest rates based on risk to the applicants.
•	They can take proactive measures for active applications to prevent defaults.

### Conclusion: 
Home Credit Risk default capstone project was thoughtful project, which referred as a practice for the next semester Final project to present to sponsors. It really helped me in understanding how machine learning methods work in real time. The professors weekly online demonstration on each session and example code and git hub portfolio links they provided gave me a step-by-step idea on working on the project.  I’m happy about the progress I made throughout the course duration in understanding and working on concepts such as cleaning the data, data manipulation, Hypothesis testing, Feature selection and scaling, Modeling and Tuning, sampling techniques and finally interpreting the results in business perspective. Working in teams for modeling helped to dig deeper into the modeling and feature engineering for improving the model’s performance. Each of us have worked together in selection of models and tuning them to get the best optimal performance, the workload has been distributed. I appreciate the opportunity to grow and learn from my teammates. Overall, I am confident that this experience will help me to have a solid foundation for success in the field of Data Science and future projects.

	
