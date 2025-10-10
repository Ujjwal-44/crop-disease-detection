📘 Plant and Crop Disease Detection using Machine Learning Models
Abstract

Timely detection of crop and plant diseases is crucial for ensuring agricultural productivity and food security.
This project presents a machine learning-based approach for detecting crop diseases using ensemble models, primarily Decision Tree and Gradient Boosting algorithms. The model is trained on agricultural datasets containing features such as environmental conditions and crop parameters. Comparative performance analysis shows that Gradient Boosting yields superior accuracy and robustness.
The system aims to assist farmers and agronomists in early diagnosis and intervention.

Index Terms

Plant disease detection, Decision Tree, Gradient Boosting, Machine Learning, Smart Agriculture.

🧩 1. Introduction

Traditional disease detection methods are often manual and time-consuming. This project addresses the challenge by applying supervised learning algorithms to predict early disease indicators through yield analysis. The models used—Linear Regression, Decision Tree Regressor, and Gradient Boosting Regressor—enable efficient identification of anomalies linked to crop diseases.

🧮 2. Methodology
Dataset and Preprocessing

The dataset includes attributes like Rainfall, Area, Crop type, State, and Lint Yield.

Missing values were handled using mean imputation.

One-hot encoding was applied to categorical variables.

Feature Selection

Target variable: Lint Yield (Pounds/Harvested Acre)

Independent variables: Encoded categorical and numerical features representing crop/environmental factors.

Machine Learning Models
Model	Description	Key Notes
Linear Regression	Assumes a linear relation between input and output	Served as a baseline model
Decision Tree Regressor	Splits data recursively to reduce mean squared error	Captured non-linear relations
Gradient Boosting Regressor	Sequentially builds weak learners to minimize residuals	Achieved best performance
📊 3. Results and Discussion

Model performance was evaluated using R² Score and Root Mean Squared Error (RMSE).

Model	R² Score	RMSE	Remarks
Linear Regression	0.65	45.2	Baseline; struggled with non-linearity
Decision Tree Regressor	0.72	38.9	Good non-linear modeling, some overfitting
Gradient Boosting Regressor	0.84	28.5	Best performance; robust and accurate

Findings:
Gradient Boosting effectively captured complex relationships among features, outperforming other models. Visualization of actual vs. predicted yields confirmed strong predictive accuracy.

🔬 4. Related Work

Previous studies such as Ferentinos (2018) and Mohanty et al. (2016) applied CNNs for leaf image classification, achieving high accuracy but requiring large datasets. Ensemble-based studies (e.g., Kamilaris & Prenafeta-Boldu, 2018) demonstrated the robustness of models like Gradient Boosting for mixed agricultural data. These findings support the use of ensemble learning for practical crop disease detection.

🚀 5. Conclusion and Future Work

Conclusion

Gradient Boosting Regressor provided the most accurate predictions with an R² of 0.84 and RMSE of 28.5.

Ensemble methods proved effective for disease-related yield anomaly detection.

Validates the potential of ML in precision agriculture.

Future Work

Integrate CNN-based image detection for leaf disease classification.

Include IoT-based sensor data (e.g., temperature, humidity, soil moisture).

Develop a web/mobile interface for farmer access.

Experiment with XGBoost and LightGBM for scalability.
