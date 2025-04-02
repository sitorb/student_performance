# Student Performance Prediction

## Overview

This project uses machine learning to predict student performance based on various factors such as study hours, previous scores, sleep, and extracurricular activities. The goal is to build a model that can accurately predict a student's "Performance Index" and provide insights into the factors influencing academic success.

## Dataset

The project utilizes a student performance dataset (`student_performance.csv`) containing information about students' study habits and academic records.  The features include:

* **Hours Studied:** The number of hours a student dedicates to studying.
* **Previous Scores:** The student's previous academic scores.
* **Extracurricular Activities:** Whether the student participates in extracurricular activities (Yes/No).
* **Sleep Hours:** The average number of hours the student sleeps per night.
* **Sample Question Papers Practiced:** The number of sample question papers the student has practiced.
* **Performance Index:** The student's overall performance index (target variable).
## Technologies Used

This project leverages the following technologies:

* **Python:** The primary programming language used for data analysis, preprocessing, model building, and evaluation.
* **Pandas:** A powerful library for data manipulation and analysis. Used for loading, cleaning, and transforming the dataset.
* **NumPy:** A fundamental library for numerical computing in Python. Used for array operations and mathematical calculations.
* **Scikit-learn:** A comprehensive machine learning library providing various algorithms, preprocessing tools, and model evaluation metrics. Used for model training, evaluation, and hyperparameter tuning.
* **Seaborn and Matplotlib:** Data visualization libraries used to create informative charts and graphs for exploring the data and presenting results.
* **Google Colab:** A cloud-based platform for running Python code and machine learning experiments. Used as the development environment for this project.

## Methodology

1. **Data Loading and Preprocessing:** The dataset is loaded using Pandas. Missing values are handled using median imputation for numerical features and 'Unknown' for categorical features. Duplicates are removed if present. Categorical features are encoded using one-hot encoding.
2. **Feature Engineering:**  Numerical features are scaled using StandardScaler and the target variable is transformed using PowerTransformer to improve model performance.
3. **Model Selection:**  A Gradient Boosting Regressor is chosen for its ability to handle complex relationships and provide accurate predictions.
4. **Model Training and Evaluation:** The model is trained using a pipeline that includes preprocessing steps. The model is evaluated using R-squared (R²) on both the training and testing sets.
5. **Hyperparameter Tuning:** The model's hyperparameters (e.g., learning rate, number of estimators) are tuned to optimize performance.
6. **Visualization:** Visualizations are generated to illustrate the relationship between features and performance, and to assess the model's predictions.

## Results

* Achieved a training R² of `0.991` and a testing R² of `0.987`.
* Developed a predictive model that can estimate student performance with reasonable accuracy.
* Generated insights into the factors influencing student academic outcomes.

## Usage

The model can be used to predict the performance of new students by providing their relevant information as input. The code includes an example of predicting performance for a new student.

## Future Work

* Experiment with other machine learning algorithms (e.g., Random Forest, Support Vector Regression) to potentially improve performance.
* Further investigate feature engineering techniques to create more informative features.
* Develop a web application or user interface to make the model accessible to a wider audience.

## Conclusion

This project demonstrates the successful application of machine learning to predict student performance. The model provides valuable insights into the factors affecting academic achievement and can be used to support students in improving their learning strategies.
