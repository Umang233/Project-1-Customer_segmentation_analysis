# project-1-Customer_segmentation_analysis

steps involved in this projects :

step 1 : Creating Problem Statement
problem statement : Customer Personality Analysis is a detailed analysis of a company’s ideal customers. It helps a business to better understand its customers and makes it easier for them to modify products according to the specific needs, behaviours and concerns of different types of customers.

step 2 : we did basic EDA only our dataset

steps in EDA
1.Checking datatype
2.checking NA value in the project (we found that there are 24 na values in INCOME column so we drop that NA values)
3.we check duplicated records 
4.we did some Visulization on our data(for undestanding the data and realationship between the columns)
5..we din some feature engineering(i.e. we created some new features from our existing features and we created new columns
6.droping some unecessary columns
6.after that we check outlier in the dataset and we found outlier in Income column and Customer_Age column so we replace that outliers by capping approch
  capping approch = in which if the outlier is present at upper extreme so we replace the outlier datapoints values with  upper extreme value and if outlier present at lower extreme then we replace that value with lower extreme value
7. we did encoding in categorical columns (i.e. "Education" column and "Living_with column)
  we have perform lebal encoding

After completing all the steps of EDA our dataset haveing 2212 rows and 24 columns

  PCA
we got lot many columns so we perform dimensionality Reduction using PCA(principal component analysis)

so after performing pca we select 3 columns which gives us 75% informtion regarding data

Clustering(Kmeans)
-->> we did clustering for making a group of similar customers
after that we have perform clusting on the data which we got from pca

after that we got our target column

**based on your clustering and targeting results, we can positioning a strategy like this:

Cluster 0 (high spending & average income): "Luxury for less".

Cluster 1 (high spending & high income): "Ultimate luxury".

Cluster 2 (low spending & low income): "Affordable products".

Cluster 3 (high spending & low income): "Affordable luxury"
**

##MODEL BUILDING

# ***There Are 3 Types of models***

  ***1.Overfitted***  --> If training accuracy is very high and testing accuracy is very low (more than 3% of difference) it is overfitted model

  ***2.Underfitted***  -->model is not able to perform good in training as well as testing it is an underfitted model

  ***3.Generalized*** -->both training accuracy and testing accuracy is high (less than 3 difference between training and testing accuracy)
-->> we use different algorithum for checking accuracy of all the model

##Model Evaluation

after compairing all the model we finalize Random_forest model 
because it given us a maximum accuracy of
 training accuracy  = 95%
 testing accuracy = 93%

##model deployment 

we created pipelines

we selected this 4 columns for deployment as this is important for prediction
Income','Recency','Customer_Age','Total_purcheses'



 



