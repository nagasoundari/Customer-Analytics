# Customer-Analytics
This is a part of my MSIM coursework and learnt different marketing strategies and techniques used.

This repository includes the following:
    1. Implementation of RFM model to pitch marketing to valued customers. 
    2. Implementation of recommendation system using Collaborative filtering approach 
    3. Implementation of recommendation system using Amazon approach. 
    4. Code samples for performing logistic and linear regression in R.
    
    
**RFM Model:** 
RFM stands for Recency, Frequency and Monetary. As the name suggests, this model uses these values as basis to predict the most valued customer. Recency is how recent a customer purchased an item, Frequency - number of times the customer had purchased and Monetary - the amount the customer has spent. The basic idea is to create bins for each of these and scoring customers against those values. This would help to identify the customers who could bring in a larger profit. Recency explains the customer’s level of engagement,
Frequency can help predict when a customer will purchase and Monetary value indicates value to the business. In general, this model is used to filter the previleged customers to target advertisements and provide with offers. 

The file [Link to RFM model](RFM_Model_R.pdf) contains the implementation of RFM model in R and also the calculation of break-even response rate.

**Collaborative Filtering Approach:**
This approach is useful when one wants to predict on preferences considering all of the long time purchase history. The basic idea is to giving weightage to other records based on their similarity with the record that we wanted to predict. For example, consider the example i have implemeted. It is to predict which movie would a particular person A rent among three available movies. In order to do this, the purchasing history of A is compared with purchasing histories of other persons say B, C and D. If B is more similar and purchased exactly the same movies as of A, then B is given higher weightage. This is done for all other users in the database. At the end, the movie selection of the persons with similar interest is recommended to person A as well.

[Link to collorative filtering](Recommendation_collaboration_filtering.pdf) contains the code snippets to perform this.


**Amazon Approach:**
Market Basket Analysis(Amazon approach) is also an approach followed to recommend products to customers. The key outputs of MBA are association rules that are statistically reliable: If event_X → event_Z. The following steps describe how to perform Market Basket Analysis.
        1. Describe items at the right “level”
        2. List the items bought in each basket
        3. Construct the N×P basket matrix, where N is the number of baskets and P is the number of products
        4. For each pair (or triplet or . . .) of products, compute
              (a) If-clause rate (or “scope”)
              (b) Confidence
              (c) Odds-ratio statistic (or “lift’)
              (d) Statistical Significance for the association
        5. If all three of the above are greater than their respective thresholds, then output the corresponding association rule
In this approach, a multivariate problem is reduced to a sequence of bivariate problems. On a nutshell, similarity between two products are calculated by S(AB) = n(AB)/squareroot(n(A)n(B)) where S(AB) is the similarity between two products A and B, n(AB) is the number of times the products A and B are purchased together, n(A) no of time product A is purchased and n(B) number of times product B is purchased. Thus by using this similarity score, place product C into recommendation “short list” if there is at least one item D in the customer’s history such that S(CD) exceeds some threshold. 

**Logistic Regression:**
[Link to logistic regression file](LogisticModel_Prediction_R.rmd) file contains the following.
A logistic regression model is built on a small dataset to calculate the 
        (a) predicted response rate, 
        (b) consequent lift (divide the predicted response rate by the average response rate in the estimation-list). 
        (c) marginal response rate 
        (d) comparison of actual vs predicted response rate


**Linear Regression:**
[Link to linear regression](Regression_types_Admetrics.pdf) contains the implementation of different linear regression models including Concave Quadratic model and concave logarithmic model (both with and without lag). This was an effective method to learn the differences between them, how to read the outputs and which method to use for different kinds of problem.

[Link to linear regression and correlation analysis](Regression_correlation_analysis_2.pdf) consists of correlation analysis between different features of a dataset and implementation of various linear regression models like simple linear model, semi-log model and log-log model.



        
        



