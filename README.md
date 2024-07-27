# Binary-Classification-of-Insurance-Cross-Selling
These are my attempts at my first kaggle playground competition. The link to the competition can be found here : https://www.kaggle.com/competitions/playground-series-s4e7/leaderboard \\

The goal of this competition is to predict the probability that someone will accept a certain insurance based on a list of 11 features. We're evaluated based on the area under the ROC curve generated by our model on a hidden test set. With four days left in the competition, the top scores are hovering around 0.89. \\

First Attempt: \\
  With my first attempt, I used the knowledge I gained from the ISLP book, as well as random snippets online. I did some basic data cleaning and feature engineering. Then I used a random forest classifier. After three submissions and some tweaking, I arrived at a score of 0.79277. 
  Pros:
    - This solution utliized libraries and methods that I was already extremely familiar with
    - Good experience in applying the skill I learned in ISLP
    - I learned the value of SMOTE and applied it on the training dataset
  Cons:
    - The score I achieved is less than desireable
    - Random Forest Classifiers don't return very precise probabilities, they're mostly estimates based on how the trees look in a neighborhood, so the approach is flawed for this use case
    - The main problem with RTC is how they were heavily overfitting on the training set. To counteract this, I tried lower the max_features, but that only marginally increased my score
  
