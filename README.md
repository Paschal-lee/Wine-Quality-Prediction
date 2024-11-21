## Description:
This project focuses on predicting wine quality based on its chemical characteristics using machine learning models. By analyzing chemical attributes such as density, acidity, and alcohol content, the study applies Random Forest, Stochastic Gradient Descent, and Support Vector Classifier to evaluate the quality of wine. The project showcases the application of machine learning in the field of viticulture.

## Objective:
To predict the quality of wine using machine learning models and identify which chemical properties have the most significant influence on the prediction.

## Dataset Used:
- <a href="https://github.com/Paschal-lee/Wine-Quality-Prediction/blob/main/WineQT.csv">Dataset</a>

## Key Questions:
What are the key chemical attributes that influence wine quality?
How well can different machine learning classifiers predict wine quality?
Which classifier provides the highest prediction accuracy for this dataset?
What insights can be derived from the chemical properties of high-quality versus low quality wines?

## Process:
Data Loading and Exploration:
Loaded the dataset WineQT.csv and explored the structure and key statistics.
Renamed columns for consistency and readability.
Checked for and handled missing values.

### Data Visualization:
Used Seaborn and Matplotlib to generate pair plots and understand correlations between features.

### Feature Selection:
Identified key chemical attributes such as Fixed Acidity, Alcohol, and Sulphates as features (X) and Quality as the target variable (y).
Data Splitting:
Split the dataset into training (80%) and testing (20%) sets using train_test_split.
Model Training:

### Trained three classifiers:
Random Forest
Stochastic Gradient Descent (SGD)
Support Vector Classifier (SVC)

### Model Evaluation:
Predicted wine quality using each classifier.
Calculated accuracy scores, precision, recall, and F1-scores.
Visualized confusion matrices for model performance evaluation.

## Insights:
### Accuracy Scores:
Random Forest achieved the highest accuracy at 69%, outperforming the other classifiers.
SGD and SVC achieved accuracies of 59% and 56%, respectively.
### Model Strengths:
Random Forest demonstrated balanced performance across classes but struggled with minority classes.
SVC showed high recall for some classes but lacked generalization.
SGD underperformed due to its sensitivity to data imbalance.

## Data Challenges:
The dataset is imbalanced, with most wines classified as quality 5 and 6. Classes like 4, 7, and 8 are underrepresented, impacting classifier performance.

## Feature Analysis:
Attributes like alcohol content and acidity showed significant influence on predicting higher wine quality.

## Conclusion:
This project illustrates the application of machine learning in wine quality prediction. Among the classifiers, Random Forest delivered the best performance, suggesting its suitability for similar tasks. However, the dataset's imbalance limits the model's ability to predict minority classes accurately. Future improvements could include:
Balancing the dataset using oversampling techniques like SMOTE.
Exploring additional models, such as XGBoost or deep learning architectures.
Conducting feature importance analysis to refine predictor selection further.
