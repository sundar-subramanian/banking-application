# Banking Application

The objective of this exercise is to analyze the banking data set to classify the customers into two groups - those who are likely to subscribe to a term deposit, and those who are not. This analysis uses historical customer data including their demographic and campaign contact characteristics as well as broader economic indicators such as consumer price index and change in employment rate. The end result is a model that canbe used by the bank to focus their marketing campaigns on those customers who are most likely to subscribe to term deposits. 

Exploratory data analysis on the data resulted in the following observations:

- Customers younger than 30 and older than 60 are more likely to sign up for term deposits.
- Students and retired persons are more likely to subscribe to term deposits.
- Single customers are more likely to sign up than married customers.
- Customers with a university degree sign up at a higher rate.
- Having a housing loan or a personal loan does not make a difference in sign up rates.
- Customers who are contacted via mobile device have higher sign up rates.
- Customers who were contacted previously have a higher change of signing up for term deposits.
- Negative change in employment rate leads to a higher sign up rate.
- Lower euribor rates result in higher sign up rates.



The analysis makes use of four classification algorithims: Logistic Regression, K-Nearest Neighbors, Decision Tree, and Support Vector Machines. All the four classifier models performed well against the training data set as measured by the accuracy rate (over 90%). However, the dataset is imbalanced, with 11% of the customers in the dataset signing up for term deposits. Precision score is a better performance metric for this dataset, as the bank would like to increase the proportion of positive identifications that actually sign up for the service. 

In terms of precision score, after some hyper parameter tuning, all four models showed a score above 65%. Of the four models, Decision Tree (with a max depth of 5) has the highest precision score of 73%.

#### Next steps

As next steps, investiage feature importance to see which features are the most relevant to the model. Apply additional tuning of hyper parameters to increase the precision score. Resampling the data to address the imbalance in the classes can be taken up. Additional data can be collected for further analysis.

Notebook located at https://github.com/sundar-subramanian/banking-application


