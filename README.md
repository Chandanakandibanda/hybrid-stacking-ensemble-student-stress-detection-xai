# Comparative Study of Stacking-Based Hybrid and Machine Learning Models for Rainfall Prediction

## About the Project

This project focuses on predicting rainfall using Machine Learning and Deep Learning techniques. It compares traditional machine learning algorithms with a proposed hybrid stacking model to evaluate their performance in rainfall prediction.

The proposed hybrid approach combines **GRU (Gated Recurrent Unit)** and **XGBoost** models, using **Linear Regression as a Meta-Learner**.

The project uses historical Indian weather data to analyse weather patterns and predict rainfall.

## Project Objectives

- Analyse historical weather data.
- Perform data cleaning and preprocessing.
- Conduct Exploratory Data Analysis (EDA).
- Identify important weather-related features.
- Develop machine learning and deep learning models.
- Implement a hybrid GRU + XGBoost stacking model.
- Compare model performance using regression evaluation metrics.

## Dataset

**Dataset:** India Weather and Rainfall Dataset

**Source:** [Mendeley Data](https://data.mendeley.com/datasets/rc5htd5dfr/1)

The dataset contains historical Indian weather observations used for rainfall prediction.

## Technologies and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- TensorFlow / Keras
- XGBoost
- Google Colab

## Machine Learning Models

The following models were implemented:

1. Linear Regression
2. Linear Support Vector Regression (LinearSVR)
3. Random Forest Regressor
4. XGBoost Regressor
5. GRU + XGBoost Stacking Model

## Proposed Hybrid Model

The proposed stacking architecture combines different learning techniques:

- **GRU:** Used to learn patterns from weather-related input features.
- **XGBoost:** Used to capture complex relationships within the dataset.
- **Linear Regression:** Acts as the meta-learner to combine predictions from the GRU and XGBoost models.

## Project Workflow

1. Dataset collection and loading
2. Data cleaning and preprocessing
3. Handling missing values
4. Exploratory Data Analysis (EDA)
5. Feature engineering
6. Data transformation and scaling
7. Model development and training
8. Hybrid stacking model implementation
9. Model evaluation
10. Results comparison and visualisation

## Evaluation Metrics

The models are evaluated using:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Percentage Error (MAPE)
- R-squared (R²)

## How to Run the Project

1. Clone this repository:

   ```bash
   git clone YOUR_GITHUB_REPOSITORY_URL
   ```

2. Open the Jupyter Notebook in Google Colab or Jupyter Notebook.

3. Download the dataset from the Mendeley Data source.

4. Upload the dataset when prompted in the notebook.

5. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn xgboost tensorflow
   ```

6. Run the notebook cells sequentially.

## Project Outcome

This project provides a comparative study of traditional machine learning algorithms and a hybrid stacking-based approach for rainfall prediction.

It explores how combining machine learning and deep learning techniques can be applied to weather forecasting problems.

## Author

**Sowjanya Vasireddy**

MSc Artificial Intelligence and Data Science

Edinburgh Napier University, United Kingdom

## Acknowledgements

I would like to acknowledge the contributors of the Indian Weather and Rainfall Dataset available through Mendeley Data, which was used for this research project.
