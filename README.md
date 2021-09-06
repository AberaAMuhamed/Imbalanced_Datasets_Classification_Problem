# Imbalanced_Datasets_Classification_Problem

## Introduction
  

 An organization XYZ provides several ways for its customers to make payments. While their service counselors can take payments over the phone, it is more cost-efficient for customers to make payments through their self-service channels such as online or through the automated phone system.  The objective is to use a predictive model to select people to receive a pre-emptive e-mail message designed to encourage them to pay online.

 The task is to build a machine learning model that predicts customers who are likely to make a service payment call in the next 5 days.




<p>  If you have spent some time in machine learning and data science, you would have definitely come across imbalanced class distribution. This is a scenario where the number of observations belonging to one class is significantly lower than those belonging to the other classes. </p>
     
        
<p> This problem is predominant in scenarios where anomaly detection is crucial like electricity pilferage, fraudulent transactions in banks, identification of rare diseases, etc. In this situation, the predictive model developed using conventional machine learning algorithms could be biased and inaccurate.    </p>
     
        
<p>
This happens because Machine Learning Algorithms are usually designed to improve accuracy by reducing the error. Thus, they do not take into account the class distribution / proportion or balance of classes. Machine Learning algorithms tend to produce unsatisfactory classifiers when faced with imbalanced datasets. For any imbalanced data set, if the event to be predicted belongs to the minority class and the event rate is less than 5%, it is usually referred to as a rare event.</p>
     
        

   
 <h5> Dataset Description: </h5>
The csv file contains data on customers who have had a bill due in the next 5 days and whether they made a service payment call. 

<p> This notebook describes various approaches for solving such class imbalance problems using various sampling techniques. We also weigh each technique for its pros and cons. Finally, I reveal an approach using which you can create a balanced class distribution and apply ensemble learning technique designed especially for this purpose.</p>

</ol>

## Challenges with standard Machine learning techniques
The conventional model evaluation methods do not accurately measure model performance when faced with imbalanced datasets.

Standard classifier algorithms like Decision Tree and Logistic Regression have a bias towards classes which have number of instances. They tend to only predict the majority class data. The features of the minority class are treated as noise and are often ignored. Thus, there is a high probability of misclassification of the minority class as compared to the majority class.

Evaluation of a classification algorithm performance is measured by the Confusion Matrix which contains information about the actual and the predicted class. However, while working in an imbalanced domain accuracy is not an appropriate measure to evaluate model performance. For example,a classifier which achieves an accuracy of 96 % with an event rate of 4 % is not accurate, if it classifies all instances as the majority class. And eliminates the 4 % minority class observations as noise.

## Examples of imbalanced data
Apart from fraudulent transactions, other examples of a common business problem with imbalanced dataset are:

- Datasets to identify customer churn where a vast majority of customers will continue using the service. Specifically, Telecommunication companies where Churn Rate is lower than 2 %.
- Data sets to identify rare diseases in medical diagnostics etc.
- Natural Disaster like Earthquakes
