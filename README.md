# Optimizing Predictive Performance: A Logistic Regression Approach for Accurate Target Prediction

## Project Overview

This project focuses on evaluating multiple logistic regression models to predict a target variable based on various feature sets. The models are tested using performance metrics such as accuracy, precision, recall, ROC AUC, and cross-validation scores. The business case revolves around selecting the best predictive model for deployment, balancing interpretability and computational efficiency while maintaining high predictive performance.

## Business Case

The business objective is to predict a target variable accurately and efficiently, with an emphasis on maximizing model performance in real-world scenarios. By evaluating three different models, each with varying feature sets, the goal was to identify the most reliable model that can deliver accurate predictions. This model will then be used to support business decision-making processes, enabling data-driven strategies for future actions.

## Steps Taken to Solve the Problem

### 1. **Data Preparation and Preprocessing**
   - **Feature Engineering**: Three feature sets were prepared:
     - **Model 1**: Logistic regression with all available features.
     - **Model 2**: Logistic regression with PCA (Principal Component Analysis) features to reduce dimensionality.
     - **Model 3**: Logistic regression with manually selected features.
   - **Data Splitting**: The dataset was split into training and testing subsets for model evaluation.

### 2. **Model Building**
   - Trained three separate logistic regression models using different feature sets:
     - **Model 1**: Logistic regression with all features.
     - **Model 2**: Logistic regression with PCA-reduced features.
     - **Model 3**: Logistic regression with manually selected features.

### 3. **Model Evaluation**
   - Each model was evaluated using the following metrics:
     - **Accuracy**: The percentage of correctly predicted outcomes.
     - **Precision**: The proportion of positive predictions that were actually correct.
     - **ROC AUC**: The area under the Receiver Operating Characteristic curve, indicating the model's ability to distinguish between classes.
   - The models were evaluated on a test set to assess their performance on unseen data.

### 4. **Cross-Validation**
   - Cross-validation was performed for Model 1 using 5-folds to assess its stability and reliability.
   - The cross-validation scores confirmed the robustness of Model 1, with high accuracy across all folds.

### 5. **Testing the Best Model**
   - The best-performing model (Model 1) was evaluated on the testing dataset, providing metrics like accuracy, precision, recall, and F1-score.
   - The model was confirmed to have high accuracy and a balanced performance in correctly identifying both positive and negative instances.

### 6. **Model Comparison and Selection**
   - A comparison of all three models based on the evaluation metrics indicated that:
     - **Model 1** (with all features) outperformed the others with the highest ROC AUC score (96.65%).
     - **Model 2** showed a good balance of accuracy, precision, and ROC AUC (93.94%).
     - **Model 3** had the weakest performance across all metrics.
   - **Final Decision**: Model 1 was selected as the most effective model for deployment based on its superior performance across multiple metrics.

## Key Findings

- **Best Model**: Model 1 (Logistic Regression with all features) was the best-performing model with a high ROC AUC score and strong precision and accuracy.
- **Model Stability**: Cross-validation demonstrated the consistency and robustness of Model 1.
- **Testing Performance**: Model 1 achieved high accuracy (94.12%) and strong precision and recall when tested on the unseen dataset.
- **Alternative Models**: Model 2, though slightly lower in performance, could be used in scenarios where a balance between interpretability and performance is important.

## Business Recommendations

1. **Deploy Model 1**: Given its superior performance, Model 1 should be deployed for real-time predictions. Its high ROC AUC score ensures that it distinguishes well between the target classes, making it a reliable choice for decision-making.
2. **Consider Model 2 for Interpretability**: If interpretability is a priority, Model 2 provides a good trade-off, though it performs slightly lower in terms of overall metrics.
3. **Model 3**: This model should be used only for exploratory purposes or when working with specific, manually selected features that may have additional business relevance.

## Conclusion

This analysis demonstrates the importance of evaluating multiple models and selecting the one that aligns best with business needs. By focusing on performance metrics such as ROC AUC, accuracy, and precision, the best model was identified and selected for deployment. Further testing and evaluation will ensure that the model continues to perform well in real-world applications.

---

### Author

Ansuman Patnaik  
MS in Data Science & Analytics, Yeshiva University  
Email: ansu1p89k@gmail.com
