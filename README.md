# Loan-status-Prediction
Loan Approval Prediction using Decision Tree,Random Forest and K fold cross validation.
Steps followed
1.  Clean the dataset by removing any rows/columns with missing values. Include an explanation for each removed row/column and the number of missing values in it.
2.  Randomly split the data into K equal folds. Set K= 5. For example, if the dataset contains 10,000 rows, randomly split it into 5 parts, each containing 2,000 rows. Use the Startified K FoldLinks to an external site. function for generating the random splits. 
3.  Create a for loop that passes over the 5 folds, each time it 4 folds for training a decision tree classifier and the remaining fold for testing and computing the classification accuracy. Notice that each iteration will use a different fold for testing.
    1.  With each train-test 4-1 split, create a parameter grid that experiments with 'gini' & 'entropy' impurity measures.
    2.  Make sure that the maximum tree depth is set to a value high enough for your dataset. You will not really fin-tune this parameter. Just set to a some high value. You can set it equal to 10 times the number of attributes (columns) in your dataset. 
    3.Notice that each split-impurity measure will generate one accuracy value. That is, the total number of generated accuracies are 5 * 2 = 10
4.  Compute the overall accuracy for Gini by averaging over the 5 runs over the 5 folds that used Gini. Likewise compute the overall accuracy for Entropy.
