# KNN Classification for Marketing Campaign Analysis

## Project Overview
This project leverages the K-Nearest Neighbors (KNN) algorithm to predict customer responses in a marketing campaign. The goal is to classify whether a customer will respond positively (Response = 1) or negatively (Response = 0) based on demographic and behavioral data. The project features extensive data preprocessing, exploratory data analysis (EDA), and model performance evaluation.

## Contents
- Data Import and Preprocessing
- Exploratory Data Analysis (EDA)
- Model Building and Hyperparameter Tuning
- Key Findings and Performance Metrics

## Data Overview
The dataset comprises:
- **Demographic features**: Income, Marital Status, etc.
- **Behavioral responses**: Purchase behavior in response to the marketing campaign.

### Data Preprocessing
- Addressed missing values in the `Income` field.
- Normalized the features for KNN to ensure balanced distance calculations.

## Exploratory Data Analysis
- Investigated demographic characteristics of customers who responded positively versus negatively.
- Visualized the relationship between features such as marital status, income, and campaign response.

## Model Building
- The KNN model was developed and fine-tuned using different hyperparameter configurations:
  - **Metric**: Euclidean distance
  - **Weights**: Uniform and distance-based weighting
  - **Range of \( k \)**: Values from 1 to 30 were tested to optimize performance.

## Results and Evaluation
![image](https://github.com/user-attachments/assets/c70e51ae-9deb-441a-a9cc-1b8924367e15)

- **Optimal \( k \)**: The best validation accuracy was observed at \( k = 6 \) using uniform weights.
- **Performance Metrics**:
  ![image](https://github.com/user-attachments/assets/0f69057c-f731-4065-a900-2fc6e84d4d6e)

  - **Validation Accuracy at \( k = 6 \)**
  - Accuracy trends showed that increasing \( k \) generally improved stability but could reduce precision for larger \( k \) values.

## Key Findings
![image](https://github.com/user-attachments/assets/12941723-4700-40bf-a283-c5d33f1d993c)

1. **Feature Importance**: Income and marital status were significant predictors of customer response.
2. **Accuracy Trends**: The model's performance varied significantly with \( k \), emphasizing the importance of hyperparameter tuning.

## Conclusion
The KNN model provides actionable insights into the factors influencing customer response, which can be leveraged to optimize marketing strategies. The exploration and results highlight the critical role of feature selection and hyperparameter optimization in achieving robust model performance.
