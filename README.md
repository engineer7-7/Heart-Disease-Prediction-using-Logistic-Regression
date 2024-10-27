Heart Disease Prediction Project
This project uses machine learning techniques to predict the 10-year risk of heart disease based on various health factors. The model is trained on the Framingham Heart Study dataset, and we utilize Logistic Regression as the primary model for prediction.

Project Structure
Data Loading and Exploration
Data Cleaning and Preprocessing
Data Visualization
Dataset Splitting
Model Training
Model Evaluation
Steps
1. Data Loading and Exploration
Dataset: framingham.csv
Columns and Rows: We check the dimensions of the dataset to understand the structure and inspect a sample of the data.
2. Data Cleaning and Preprocessing
Dropping Irrelevant Columns: We drop the education column since it is not relevant to heart disease prediction.
Handling Missing Values: Columns with missing values are filled with the mean of each column to maintain data integrity.
3. Data Visualization
To better understand the relationship between various features and the target variable (TenYearCHD), several plots are created:

Heart Disease by Gender: Displays the probability of heart disease for the next 10 years by gender (0 = women, 1 = men).
Heart Disease by Age: Shows heart disease prediction by different age groups.
Heart Disease by Smoking Status: Analyzes the relationship between smoking status and heart disease risk.
4. Dataset Splitting
Features (X): All columns except the target column TenYearCHD.
Target (y): The column TenYearCHD.
Train-Test Split: The dataset is split into training and testing sets (80% train, 20% test) for model evaluation.
5. Logistic Regression Model
A Logistic Regression model is trained on the training set to predict the 10-year heart disease risk.

Model Parameters: max_iter=10000 is used to ensure convergence.
6. Model Evaluation
We evaluate the model's performance using various metrics:

Accuracy: The proportion of correct predictions out of total predictions.
F1 Score: Harmonic mean of precision and recall, useful for imbalanced datasets.
Classification Report: Contains precision, recall, and F1-score for each class.
Confusion Matrix: Visualizes the performance of the model in distinguishing between classes.
Visualizations
Heatmap of Confusion Matrix: A heatmap is created to visualize the confusion matrix, showing how well the model distinguishes between positive and negative cases of heart disease.
Requirements
Python 3.x
Libraries: pandas, numpy, matplotlib, seaborn, sklearn
