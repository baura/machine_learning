#This is my project for Machine Learning course from the Data Science specialization of Coursera.

##I proceeded as follows:
1. Download the csv files and call them *training* and *testing*, respectively;
2. Correct the values like #DIV0!, turning them into NA's;
3. Divide the training set into *train_train*, for 70% of its observations, and *test_train*;
4. Check how many columns have more than 90 % of observations missing and kick them out. I made sure that most of these NA's values are such for 
most of these columns;
5. Looked at the distribution of each numeric variable of those remained (55), subdivided by their *classe* value;
6. Performed principal component analysis, as many variables showed high collinearity;
7. Played around with classification methods on the preprocessed *train_train* subset and looked at the accuracy on predicting the outcome *classe* on *test_train* (preprocessed with the same rotation as in *train_train*);
8. All those methods with an accuracy higher than 0.5 were then used in a combined predictor that worked as a "majority vote". Recall that, having 5 levels of *classe*, a random predictor would have 0.2 accuracy;
9. Use this combined predictor to predict *classe* in *testing*.
