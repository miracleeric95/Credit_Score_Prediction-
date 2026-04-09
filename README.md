# Credit_Score_Prediction-
Credit scoring algorithms, which make a guess at the probability of default, informing banks use to determine whether or not a loan should be granted
## Problem Statement:
Develop a predictive system to identify whether or not customers are credit worthy and are not at serious delinquencyfor condidearation for load.
## Procedure
Install and import the following dependencies
import pandas as pd
import matplotlib.pyplot as plt
%matplotlib inline
import numpy as np
import seaborn as sns
from sklearn.preprocessing import LabelEncoder, MinMaxScaler,StandardScaler
from sklearn.model_selection import train_test_split
from sklearn.neighbors import KNeighborsClassifier
from sklearn.metrics import classification_report, confusion_matrix, accuracy_score,roc_auc_score
from sklearn.ensemble import RandomForestClassifier
from sklearn.tree import DecisionTreeClassifier
import xgboost as xgb
import warnings
warnings.filterwarnings('ignore')
## Dataset Exploration
The dataset was explored using heatmap,barchat , boxplot,scatter plot,count plot,and density map
# Data Cleaning
The unamed :0 which is column [0] was dropped from the dataset since it does not have any much impact on the prediction of the model
The standard Scaler was used to transform the dataset in order to do away with extreme values that could hinder the perfomance of the model
# Model Result
The KNeighbours classier gave an accuracy of 93.30% and auc of 54.73%. 
The Decision Tree clasffier gave an accuracy of 99.97% and auc of 99.99%
The XGBoost  gave an accuracy of 93.96% and auc of 99.99%
Finally, RandomForest gave an accuracy of 99.96% and auc of 99.99%
The best performing model from the metrics is the Decision Tree. It has highest accuracy and auc scores combined.
# Files
The dataset used is in the file labeled as archive.zip and the python file in Credit_Score_Predict_Group_3
