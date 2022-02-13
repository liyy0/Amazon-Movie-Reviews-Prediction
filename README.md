# Star Rating Prediction of Amazon Movie Review

## Main Goal of the Project
Nowadays, a massive amount of reviews is available online. Besides offering a valuable wording review, it always comes with a rating from 0 to 5 stars. The goal of this project is to predict the star rating associated with user reviews from Amazon Movie Reviews using the available feature.

## Data Fields:
1. ProductId - unique identifier for the product
2. UserId - unique identifier for the user
HelpfulnessNumerator - number of users who found the review helpful
3. HelpfulnessDenominator - number of users who indicated whether they found the review helpful
4. Score - rating between 1 and 5
5. Time - timestamp for the review
6. Summary - brief summary of the review
7. Text - text of the review
8. Id - a unique identifier associated with a review

## Model Applied
Before appling models, I applied some common NLP model to turn words into numeric matrix and clean the data, including Vectorizing the word and finding the stem of each English words.
I applied 4 different model onto the dataset: KNN, Naive Bayes, SVM and Logistic Regression and made some adjustment and evaluation based on their performances.
1. `predict-constant.py` to predict the same score for all rows in the test set
2. `predict-knn.py` to predict the score using KNN
3. `Naive Bayes.ipynb` to predict the score using KNN
4. `SVM.ipynb` and `SVM_COMBINE.ipynb` to predict the score using svm model on either only Text or the combination of Text and other feature like Summary
5. `Logistic-Regression.ipynb` to predict the score using Logistic-Regression 

## Short Summary
In general, Naive Bayes is a good way to start the prediction project since it creats a relatively precise prediction in a short time. But Logistic Regression have best performances when you increase the iteration. However, it requires a long time to preduce the outcome.
More detailed comparison are in the `Report_liyy.pdf` file.

## Dataset Citation

J. McAuley and J. Leskovec. From amateurs to connoisseurs: modeling the evolution of user expertise through online reviews. WWW, 2013