# Parkinson-Disease-prediction-using-ensemble-learning-and-XAI


### Introduction
Parkinson’s Disease (PD) is a chronic and progressive neurodegenerative disorder that primarily affects motor function due to the loss of dopamine-producing neurons in the brain. Early diagnosis is crucial for effective treatment planning and improved quality of life. However, due to the complexity and subtlety of early symptoms, accurate diagnosis remains a challenge. In this work, we propose a robust machine learning framework that leverages ensemble learning techniques combined with Explainable Artificial Intelligence (XAI) to predict Parkinson’s Disease and offer interpretable insights into the model’s decisions.

### Ensemble Learning for Robust Prediction
Ensemble learning involves combining the predictions of multiple base models to produce a stronger, more reliable prediction system. In our approach, we employ various ensemble methods such as:

Stacking: combining multiple base models with a meta-learner

This method help reduce overfitting, improve generalization, and boost predictive accuracy, especially when working with biomedical datasets that may contain noise or imbalanced samples.

### Dataset and Features
We utilize a structured biomedical dataset containing voice measurements and biomedical voice features (e.g., jitter, shimmer, HNR, and pitch-related features) from patients diagnosed with PD and healthy individuals. The dataset is preprocessed through normalization, feature selection, and missing value handling to ensure optimal model performance.

### Integration of Explainable AI (XAI)
While ensemble models provide high accuracy, they often lack transparency. To address this, we incorporate Explainable AI technique:

SHAP (SHapley Additive exPlanations): Quantifies each feature's contribution to the final prediction, providing a global and local understanding of the model.

These tools not only increase model interpretability but also help clinicians validate predictions based on medical reasoning.

### Results and Analysis
The ensemble models, particularly Random Forest and XGBoost, demonstrated superior performance in terms of accuracy, precision, recall, and F1-score compared to individual classifiers. SHAP and LIME visualizations revealed that features like MDVP: Fo(Hz), spread1, and PPE had significant influence in distinguishing between PD patients and healthy individuals.

### Conclusion
The integration of ensemble learning and XAI provides a powerful and trustworthy approach to Parkinson’s Disease prediction. It not only enhances diagnostic performance but also ensures interpretability, making it suitable for real-world clinical decision support systems. Future work may include incorporating deep learning models and testing on multimodal data for further performance gains.
