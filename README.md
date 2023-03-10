# Marketing-Campaign-Analysis

Marketing campaigns are one of the popular methods to adopted by banks to enhance their business and increase their custormers. Use of direct marketing when customer segmentation is known is still widely used by many Banks. Telemarketing, digital marketing etc utilize remote interactions through a contact center or digital media respectively. Such direct campaigns can be improved in their efficiency through the use of data-driven business intelligence tools.

In this analysis we are provided with a data-set  form UCI Machine Learning repository) that contains marketing campaign results of a Portuguese bank with ~41,000 candidates profile with 20 features to predict the success of the future campaigns. For this data-centric business problem, we propose utilization of various classification model(s)  (K-nearest neighbors (KNN), Logistic regression (LR), Decision trees(DT), Support vector machines(SVM)) to predict the candidates response class as 'success' if the campaign is accepted or else 'failure'. 

We utilized the subset of the features presented to us to know the effectiveness of the four models so that models with good performance could be put to use for predictions with the data will all the features. We evaluated the models based on F1 score and area of the receiver operator characteristic curve (ROC-AUC score). Recall was utilized to choose between models with comparable performances. We randomly split the data available with 20% of the data serving as the development dataset to test the model along with stratification of the two classes of the response variable for balanced representation in both training and development set.

Logistic regression and decision trees evaluated to 0.38, 0.78 and 0.46, 0.80 of F1 and ROC-AUC scores respectively. We also evaluated these models with and without balancing the weights for the classes due to inherent unbalance in representation of 'success' class in the data. The LR and DT models with weighted balances consistently evaluated with higher recall score. 

DT model presented itself with the best results (AUC=0.79,F1=0.46, recall=0.62) in all evaluation metrics of allowing to reach ~80% of the subscribers by selecting half of the better classified clients. Further analysis on importance of features along with knowledge extraction from domain can be compared to validate the credibility and valuabilty of these models. 

key words: Marketing, Sales, Classification, Logistic regression, Decision tree, F1 score, ROC-AUC

Link to Notebook: https://github.com/R-Madhuram/Marketing-Campaign-Analysis/blob/main/prompt_III.ipynb
