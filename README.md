Meli Customer Behavior Prediction

This project aims to predict customer purchasing behavior using machine learning models on a dataset from Meli, an e-commerce platform. The project utilizes various machine learning algorithms to analyze user history and item data to forecast which items a user is likely to purchase.

Project Structure
Data Loading and Merging:

The project begins by loading the training data and item data from JSON files.
The data is then merged to create a comprehensive dataset that includes user purchase history and item details.
Feature Extraction:

User history is parsed to extract meaningful features such as the number of views, searches, and purchases.
Additional features like total view time, average view time per item, and the time span between the first and last events are calculated.
Item details such as domain_id, price, and condition are incorporated into the feature set for the most viewed item, first viewed item, and last viewed item.
Data Preprocessing:

Categorical features are encoded using LabelEncoder.
Missing values in numerical features are imputed using the median strategy with SimpleImputer.
Model Training and Evaluation:

Several machine learning models are trained and evaluated, including:
Logistic Regression
Random Forest
Extra Trees Classifier
XGBoost
LightGBM
CatBoost
Each model's performance is evaluated using metrics such as accuracy and classification reports.
Feature Importance and SHAP Analysis:

For models like XGBoost and CatBoost, feature importance is analyzed and visualized using SHAP (SHapley Additive exPlanations).
