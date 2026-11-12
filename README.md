# 🌱 Crop Recommendation System using Machine Learning

An end-to-end Machine Learning project that recommends the most suitable crop to grow based on soil composition (Nitrogen, Phosphorus, Potassium, pH) and climatic conditions (temperature, humidity, rainfall).

## 📊 Project Overview
Agricultural planning requires precise soil and weather analysis to maximize crop yield and minimize risks. This project utilizes a Random Forest Classifier trained on soil and environmental parameters to deliver highly accurate crop recommendations.

## 🛠️ Dataset & Features
The dataset (`crop_prediction.xlsx`) contains **2,200 records** across 8 key features:
- **N, P, K:** Ratios of Nitrogen, Phosphorus, and Potassium in the soil.
- **Temperature:** Ambient temperature in degrees Celsius.
- **Humidity:** Relative humidity percentage.
- **pH:** Soil pH value.
- **Rainfall:** Rainfall amount in millimeters.
- **Label:** The target crop category (e.g., rice, maize, cotton, banana, coffee, watermelon, etc.).

## 🔍 Data Cleaning & Exploratory Data Analysis (EDA)
- **Missing Value Imputation:** Handled missing values in the Nitrogen (`N`) column by filling with `0` and in the `humidity` column by filling with the column mean.
- **Statistical Insights:** Examined feature distributions, data skewness, and correlation matrices to understand soil-climate dependencies across different crop types.

## 🤖 Model Training & Evaluation
- **Train-Test Split:** Split the dataset into an **80% training set** and a **20% testing set** (`random_state=0`).
- **Algorithm:** Trained a **Random Forest Classifier** (`RandomForestClassifier`).
- **Performance:** Achieved an exceptional overall accuracy score of **99.32%** on test data, validated via a confusion matrix and detailed classification report (precision, recall, and f1-score).

## 💻 Tech Stack & Libraries
- **Python**
- **Pandas & NumPy** (Data manipulation & array processing)
- **Scikit-Learn** (Model building, train-test splitting, Random Forest, evaluation metrics)
- **Matplotlib & Seaborn** (Data visualization, distribution plots, and correlation heatmaps)

## 📂 Repository Structure
- `/data` — Contains the raw dataset (`crop_prediction.xlsx`).
- `/notebook` — Contains the Jupyter Notebook (`Crop_Recommendation_System.ipynb`) detailing data cleaning, EDA, and model training.
- `/materials` — Contains supplementary reference materials

---
*Created as part of a professional data science portfolio.*
