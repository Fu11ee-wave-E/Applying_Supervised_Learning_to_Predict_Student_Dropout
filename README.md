# Applying Supervised Learning to Predict Student Dropout

<div align="justify">
  
## Objectives 
The project involves comprehensive data exploration, preprocessing, and feature engineering to ensure 
high-quality input for the machine learning (ML) models. Multiple predictive algorithms, such as 
XGBoost, and a neural network-based model, are employed and compared to determine the most effective 
approach for predicting student dropout.

## Background 
A tabular dataset was studied to predict student dropout using two supervised ML approaches: 
eXtreme Gradient Boosting (XGBoost) and a neural network (NN) model. The dataset contained demographic 
and administrative records of over 25,000 international students. To predict student dropout, the dataset 
was pre-processed and analysed in three distinct stages, each reflecting the real-world 
progression of data acquisition: 

1. Applicant and course information 
2. Student and engagement data 
3. Academic performance data 

## Data Pre-processing 
The processing steps included: 
* Removal of features with high cardinality (> 200) and high percentages of 
missing values (> 50%) were removed. 
* Imputing missing values of numerical features via the median. 
* One-hot and ordinal encoding of categorical features where applicable. 
* Assessment of the target variable for class imbalance. 
* Standard scaling of continuous numerical features, to improve model performance and preserve
interpretability across the encoded categorical variables.

*Before model training, a train-test split of 80-20% was applied, followed by a 10% split of 
the training dataset as the validation dataset. Stratification was implemented in both 
splits to address the class imbalance.*

## Study Design
Following data processing at each stage, a baseline XGBoost and a NN model was 
instantiated and hyperparameter tuned. The tuned model at a given stage formed the 
baseline model of the next as depicted in the figure below.

<br><br>
<p align="left">
  <img src="Figures/OCSVM_IsoForest.png" height="700">
</p>
<br><br>

</div>
