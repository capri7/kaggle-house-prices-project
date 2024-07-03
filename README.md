# Kaggle House Prices Prediction

This repository contains code and resources for predicting house prices using machine learning techniques. This project was developed as part of the Kaggle competition "House Prices - Advanced Regression Techniques".

## Overview

In this project, we use various machine learning algorithms to predict the final price of houses based on various features. The dataset contains features such as the size of the house, the number of rooms, the year it was built, and more.

## Requirements

To run this project, you need the following dependencies:
- Python 3.8+
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- jupyter

You can install the required packages using `pip`:

```bash
pip install -r requirements.txt

Notebooks Overview
Train Data Preprocessing
1_1_trainデータの前処理_不要な列の削除__データ型の変換__補完__削除.ipynb: Removing unnecessary columns, converting data types, filling and dropping missing values.
1_2_trainデータの前処理_異常値の検出と処理.ipynb: Detecting and handling outliers.
1_3_trainデータの前処理_新しい特徴量の作成.ipynb: Creating new features.
1_4_trainデータの前処理_カテゴリ変数のエンコーディング.ipynb: Encoding categorical variables.
1_5_trainデータの前処理_数値変数のスケーリング.ipynb: Scaling numerical variables.
1_6_trainデータをRandomForestでトレーニングし評価する.ipynb: Training and evaluating the RandomForest model.
1_7_trainデータのモデルが重視している特徴量の確認.ipynb: Checking the important features as identified by the model.
Test Data Preprocessing
2_1_testデータの前処理_不要な列の削除__データ型の変換__補完__削除.ipynb: Removing unnecessary columns, converting data types, filling and dropping missing values.
2_2_testデータの前処理_異常値の検出と処理.ipynb: Detecting and handling outliers.
2_3_testデータの前処理_新しい特徴量の作成.ipynb: Creating new features.
2_4_testデータの前処理_カテゴリ変数のエンコーディング.ipynb: Encoding categorical variables.
2_5_testデータの前処理_数値変数のスケーリング.ipynb: Scaling numerical variables.
2_6_testデータの予測とファイルの提出.ipynb: Making predictions and preparing the submission file.
Feature Engineering
In the feature engineering step, we created new features such as:

TotalArea: Sum of GrLivArea, TotalBsmtSF, and GarageArea
QualityScore: Sum of quality-related features (OverallQual, ExterQual, KitchenQual, BsmtQual, HeatingQC)
And more...
For more details, refer to the 1_3_trainデータの前処理_新しい特徴量の作成.ipynb notebook.

Model Training and Evaluation
We trained several machine learning models including Random Forest, XGBoost, and LightGBM. The best performing model was a Random Forest with the following parameters:

max_depth: 10
max_features: 'sqrt'
min_samples_leaf: 1
min_samples_split: 5
n_estimators: 100
For more details, refer to the 1_6_trainデータをRandomForestでトレーニングし評価する.ipynb notebook.

Results
The final model achieved a Mean Absolute Error (MAE) of 15436.2778 and an R-squared (R2) of 0.9018 on the test set.

Future Work
Further tune the hyperparameters of the models.
Explore additional feature engineering techniques.
Try different ensemble methods to improve the prediction accuracy.
Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.
