# Classification-on-Wine-DATA-SET
------------------------------------------------------------------------------------------------------------------------------
Used Decision Tree and Support Vector Machine on Wine Dataset for classification. Interpreted, predicted, visualized and compared the 
results among the classifiers using Scikit-learn, NumPy, Pandas and Matplotlib. 
Loaded the dataset from sklearn and split it for training the model and then testing the model on unseen data.
Used confusion matrix and classification report for measuring the accuracy of the prediction by the model.

----------------------------------------------------------------------------------------------------------------------------------
WINE DATASET

The data is the results of a chemical analysis of wines grown in the same region in Italy by three different cultivators. 
There are thirteen different measurements taken for different constituents found in the three types of wine.

This dataset has been imported from scikit-learn
Data Set Characteristics:
  •	Number of instances: 178 (50 in each of three classes)
  •	Number of attributes: 13 numeric, predictive attributes and the class
Attribute information:
  1.	Alcohol
  2.	Malic Acid
  3.	Ash
  4.	Alcalinity of ash
  5.	Magnesium
  6.	Total Phenols
  7.	Flavonoids
  8.	Nonflavonoid phenols
  9.	Proanthocyanins
  10.	Color intensity
  11.	Hue
  12.	OD280/OD315 of diluted wines
  13.	Proline
Class: 
1.	 class_0
2.	 class_1
3.	 Class_2

•	Missing attributes values: None

•	Creator: R.A Fisher
------------------------------------------------------------------------------------------------------------
Report For DECISION TREE:
  Decision Trees (DTs) are a non-parametric supervised learning method used for classification and regression. The goal is to create a
  model that predicts the value of a target variable by learning simple decision rules inferred from the data features.

Comparison for Gini & Entropy:
  MEAN ACCURACY
    •	0.9629629629629629 is the mean accuracy for DT from Gini
    •	0.9074074074074074 is the mean accuracy for DT from entropy

    This states that Gini has a better mean accuracy for the DT


 CONFUSION MATRIX
  GINI: [17 1 0]               ENTROPY: [17 1 0]
       [1 20 0]                        [3 18 0]
       [0 0 15]                        [0 1 14]

   AS we notice from the confusion matrix that the Gini criteria gives us more true result than entropy.
------------------------------------------------------------------------------------------------------------------------------------
Report For SVM:
  SVM are a set of supervised learning methods used for classification, regression and outliers detection. SVM offers very high accuracy
  compared to other classifiers such as logistic regression, and decision trees. It is known for its kernel trick to handle nonlinear 
  input spaces. It is used in a variety of applications such as face detection,intrusion detection, classification of emails, news 
  articles and web pages, classification of genes, and handwriting recognition.
  
  Comparing the results:
    PREDICTION OF THE WINE DATASET:
      FOR LINEAR:
        [2 1 2 1 0 0 1 1 1 2 2 0 1 0 2 1 0 0 1 2 0 1 0 0 1 2 2 0 0 0 1 1 1 1 2 0 2 1 1 2 0 2 0 0 0 1 1 2 1 0 1 0 0 2]
      FOR NON-LINEAR (POLYNOMIAL)
        [2 2 2 1 1 0 1 1 1 2 2 0 1 0 2 1 0 1 1 2 0 1 1 0 1 2 2 1 0 0 1 1 1 1 2 1 2 1 1 2 0 2 0 0 1 1 1 2 1 0 1 1 0 2]
      FOR NON-LINEAR (RBF)
        [2 1 2 1 0 0 1 1 1 2 2 0 1 0 2 1 0 0 0 2 0 1 0 0 1 2 2 0 0 0 1 1 1 1 2 0 2 0 1 2 0 2 0 0 0 1 0 2 1 0 1 0 0 2]
    
   CONFUSION MATRIX:
      FOR LINEAR [14 4 0]               
                 [6 14 1]                        
                 [0 2 13]


      FOR NON-LINEAR (POLYNOMIAL) [11 7 0]               
                                  [2 18 1]                        
                                  [0 1 14]


          
      FOR NON-LINEAR (RBF)  [16 2 0]               
                            [7 13 1]                        
                            [0 2 13]







