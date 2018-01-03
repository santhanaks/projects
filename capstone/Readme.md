The interesting aspect of this project is to minimize the total fraud amount that the classifier misclassifies. While this is a well studied dataset, many approaches focus on increasing accuracy of the classifier. However, the core business objective is to reduce fraud that is not detected, hence a classifier that detects all the 100 $ 1 fraudulent transactions while ignoring the one $ 2,000 fraud transaction is not effective. We accomplish this by focusing on reducing the error cost of error for the algorithm.

This project utilizes the credit card fraud dataset available at https://www.kaggle.com/dalpozz/creditcardfraud

The data consists of 30 total features [i.e. 28 principal components identified through PCA, transaction amount, time [elapsed since first transaction] along with the Class for each transaction - 1 indicating fraud and 0 indicating normal transaction. There are 492 frauds out of 284,807 total transactions in the data provided, hence this is a highly imbalanced dataset with the positive class amounting to only 0.172% of all transactions.

The project report and associated notebook examine several classifiers to determine performance using precision, recall and the total error cost. We then tune one of the classifiers (XGBoost) to improve performance and report results.
