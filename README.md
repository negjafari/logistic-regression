# Logistic Regression Binary Classifier

This project implements logistic regression from scratch in python to create a binary classifier using Breast Cancer and Ionosphere datasets. The main objectives of this project are:

- Implement logistic regression to predict the label of unseen data in Breast Cancer and Ionosphere datasets.
- Evaluate different learning rates for the logistic regression model.
- Analyze performance in terms of both speed and precision across two datasets.
- Investigate whether selecting a subset of features or adding new features could enhance the model's accuracy.

## Dataset Description

- **Breast Cancer Dataset**: The target variable represents the diagnosis (M = malignant, B = benign).
- **Ionosphere Dataset**: The target variable, denoted as 'g' (good signal) or 'b' (bad signal.

![image](https://github.com/negjafari/logistic-regression/assets/59292708/0539d589-f80f-4074-a945-c434f2289cd1)

Distribution of the two classes for both datasets

## Evaluation of Model Accuracy

1. **Adding New Features**:
   - Perform correlation analysis to calculate the correlation of each feature with the target variable.
   - Features with a high absolute value of the correlation coefficient are considered more influential in prediction.
   - For features with high correlation value:
     - Square their value and add a new feature.
   - For features with low correlation (near zero):
     - Inverse them (1/feature) and create a new feature.
     
2. **Removing Features**:
   - Find the correlation between features.
   - For pairs of features with high correlation, select the feature with higher correlation with the target and remove the other one.

3. **Data Normalization**:
   - Normalize the data to ensure all features contribute equally to the model.

4. **Evaluation with Different Learning Rates**:
   - Assess the accuracy of the model with varying learning rates.

## Conclusion

![image](https://github.com/negjafari/logistic-regression/assets/59292708/74229b76-4c08-46a4-b741-44b68a08b295)

