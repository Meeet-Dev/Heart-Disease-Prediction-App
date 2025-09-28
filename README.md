# Heart Disease Prediction

This project predicts the risk of heart disease using machine learning models and provides an interactive web app for users to check their risk based on personal health information.

## Project Overview

Heart disease remains one of the leading causes of death worldwide. Early risk detection using data-driven models can help people take preventive action. In this project, I worked with a real-world dataset containing patient records with features such as age, sex, chest pain type, blood pressure, cholesterol, fasting blood sugar, ECG results, and more.

### Goals

- Analyze and visualize the dataset to uncover health risk patterns.
- Compare the performance of multiple machine learning classification models.
- Build an interactive Streamlit app so users can assess their heart disease risk.

## Workflow

1. **Exploratory Data Analysis (EDA):**
    - Analyzed distributions and relationships using histograms, countplots, and heatmaps.
    - Explored how factors like chest pain, age, and blood sugar relate to heart disease risk.
    - Confirmed no missing values in the dataset.

2. **Data Preprocessing:**
    - Categorical variables were encoded for model compatibility.
    - Numerical features were scaled for balanced model input.

3. **Modeling and Evaluation:**
    - Trained and tested five different classifiers:
        - Logistic Regression (Accuracy: 89.7%, F1: 0.91)
        - K-Nearest Neighbors (KNN) (Accuracy: 88%, F1: 0.89)
        - Naive Bayes (Accuracy: 88%, F1: 0.89)
        - Support Vector Machine (SVM, RBF kernel) (Accuracy: 86.4%, F1: 0.88)
        - Decision Tree (Accuracy: 75%, F1: 0.77)
    - Evaluated using accuracy and F1 score for both balanced and medical-appropriate assessment.
    - Logistic Regression performed the best overall, though KNN and Naive Bayes were close.

4. **Interactive Web App:**
    - Built with Streamlit for ease of use.
    - Users enter their health information using sliders and dropdowns.
    - The model predicts heart disease risk and returns a helpful message:
        - High risk: suggests seeing a healthcare provider.
        - Low risk: encourages staying healthy.

## How to Run

1. Install Required Library:
    ```
    pip install streamlit
    ```

2. Run the Streamlit app:
    ```
    streamlit run app.py
    ```


## Key Takeaways

- Good data prep and EDA are essential for building an accurate model.
- Comparing several algorithms helps find the most reliable approach (sometimes simpler is better for healthcare).
- Visualizations provide valuable insights and make findings understandable.
- Deploying models as web apps bridges the gap between data science and real-world use.



