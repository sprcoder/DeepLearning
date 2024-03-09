# Digit Recognizer
This a project for solving the kaggle challenge of Optiver - Trading at the close. [Kaggle Link](https://www.kaggle.com/competitions/optiver-trading-at-the-close)

## Accuracy
Acheived a MAE of 5.33 by using LighGBM and LSTM. Researched optimization of hyperparameters and the deep learning layers to include while training.

## Deep learning model developed
| Factor | LSTM | LightGBM |
|--------|------|----------|
| **Model Complexity vs. Suitability** | Complex, best for sequential data. Less effective if sequence isn't main driver. | Less complex, handles diverse data types efficiently. More suitable for stock predictions. |
| **Feature Representation** | Needs effective feature engineering for time patterns. Performance suffers if not optimal. | Autonomously uncovers complex relationships in a range of features, vital for stock predictions. |
| **Overfitting Risk** | Prone to overfitting, especially with noisy, non-stationary financial data. | Better at managing overfitting, particularly with cross-validation, leading to improved generalization. |
| **Handling Data Noise and Volatility** | May misinterpret noise as significant patterns, affected by data volatility. | Robust to noise and volatility, often leads to better performance in noisy market data. |
| **Hyperparameter Tuning** | Performance heavily depends on tuning. Poor tuning leads to lesser performance. | Performance heavily influenced by hyperparameters. Well-tuned models perform better. |
| **Data Training and Validation** | Lacks robust validation, effectiveness may not be accurately assessed. | Benefits from 5-fold cross-validation, ensuring reliable performance estimation. |
| **Simplicity and Interpretability** | Complexity can be a drawback in less complex scenarios. Less interpretable. | Simpler and more interpretable, aiding in better tuning and performance. |