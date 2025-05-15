# 🌧️ RainCast AI – Rainfall Prediction Using Machine Learning

RainCast AI is a data science project that predicts whether it will rain tomorrow in the Melbourne area using historical weather data. This project walks through an end-to-end machine learning pipeline—from data preprocessing and feature engineering to model training, evaluation, and feature importance analysis.

## 📊 Project Description

This project leverages Australian weather data to classify the likelihood of rainfall the next day. We compare the performance of two popular classifiers: **Random Forest** and **Logistic Regression**. The pipeline includes data cleaning, seasonal mapping, encoding, scaling, model selection using GridSearchCV, and result visualization.

## 🛠️ Technologies Used

- Python 3
- pandas, numpy
- scikit-learn
- matplotlib, seaborn
- Google Colab

## 📁 Dataset

The dataset includes historical weather observations for various Australian locations, including:

- Temperature, humidity, pressure
- Wind direction/speed
- Sunshine and evaporation levels
- Binary target column: `RainTomorrow` (Yes/No)

## 🧪 Steps Followed

1. **Data Preprocessing**
   - Converted `Date` to `Season`
   - Handled categorical and numeric columns
   - Dropped irrelevant or redundant columns

2. **Exploratory Data Analysis**
   - Class distribution check (imbalanced)
   - Visualization of key metrics

3. **Model Training**
   - Trained with `RandomForestClassifier` and `LogisticRegression`
   - Used GridSearchCV with cross-validation
   - Evaluated using accuracy, F1-score, confusion matrix

4. **Feature Importance**
   - Extracted and visualized top features impacting prediction

## ✅ Results

- **Random Forest**
  - Accuracy: ~84%
  - True Positive Rate (Yes Rain): ~50%
- **Logistic Regression**
  - Accuracy: ~83%
  - True Positive Rate (Yes Rain): ~51%

📌 **Conclusion**: While both models performed similarly, Random Forest offered slightly better precision overall, but Logistic Regression achieved a marginally higher true positive rate for rain prediction.

## 📉 Most Important Features

- Humidity at 3pm
- Pressure at 3pm and 9am
- Sunshine hours
- WindGustSpeed

## 📌 How to Run

1. Clone the repository or open the notebook in Google Colab.
2. Install required packages.
3. Run each cell sequentially to replicate the full pipeline.

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

## 📬 Contact

For any inquiries or suggestions, please reach out to [Your Name or GitHub handle].
