# deep-learning-challenge
deep-learning-challenge

1.	Introduction

Exploration various strategies to optimize a deep neural network model to achieve a target predictive accuracy of over 75% on a charity dataset was conducted. The steps followed were data preprocessing, feature engineering, model architecture adjustments, and hyperparameter tuning. This document outlines the methodologies used, results obtained, and insights gained from the process.

2.	Data Preprocessing

•	Initial Data Loading and Cleaning

We begin by loading the dataset and performing initial cleaning steps. The dataset includes several features, some of which may not be beneficial for our predictive model. The initial steps include dropping unnecessary columns and handling missing values.

•	Binning Rare Occurrences

To handle categorical features with many rare occurrences, we bin these rare occurrences into a single category labeled "Other". This helps reduce noise in the data.


•	One-Hot Encoding

We then convert categorical variables to numerical format using one-hot encoding, ensuring all features are in a suitable format for modeling.


3.	Feature Engineering
•	To identify the most relevant features, we use feature importance from a Random Forest classifier. This helps in reducing the feature space to only the most significant features.


4.	Model Architecture
•	Initial and further models were defined with an input layer, hidden layer and output layers.  Model then compiled using binary crossentropy and the Adam optimizer.

5.	Hyperparameter Tuning 
•	Grid search was used to find the best combination of hyperparameters, including optimizer and learning rate

6.	Early Stop
Early stopping implemented to prevent overfitting by monitoring the validation loss and stopping training when it ceases to improve.


7.	Evaluation and Results
After training the model’s performance was evaluated on the test data. Despite the efforts and time take to tune up for best model, the accuracy rate only reached to 72.58% which was below the target of 75%. 


Conclusion
Even though exploration of various techniques and several iterations & improvements in data preprocessing for the optimization of neural network model to predicting charity outcomes, accuracy was only limited to 72.58%. Further optimization with additional feature engineering and ensemble methods  might improve the model performance.
![image](https://github.com/spoudel977/deep-learning-challenge/assets/94360634/d61df2fa-222b-4930-b61b-3ccc3fc1717b)
