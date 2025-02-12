# Income_Classification
classifying wether the income of a person higher or less than 50K depending on dataset features values

## Note :the code is well documented and there is alot of blocks on it that document and summerize conclusion.Dont mess them🐲

# Income Classification Project

This project aims to classify individuals' income as either higher or lower than 50K based on various features in a given dataset.  The project follows a standard machine learning workflow, including data preprocessing, feature engineering, model training, and evaluation.

## Project Structure

The project is organized into the following sections:

1. **Data Loading and Preprocessing:**
    * Libraries:  Essential Python libraries like Pandas, NumPy, and Scikit-learn are used.
    * Correlations:  Analysis of feature correlations to understand relationships within the data.
    * Feature Engineering:  Creation of new features to potentially improve model performance.  This includes working with soil type percentages, selecting relevant features, and potentially reversing the order of data for specific analyses.  Encoding of categorical variables is also performed.
    * Final Dataframes:  The resulting preprocessed dataframes ready for model training.

2. **Model Training and Evaluation:**
    * Handling Imbalanced Data:  If the dataset exhibits class imbalance (unequal representation of income classes), techniques like oversampling or undersampling are employed.
    * Data Splitting:  The data is split into training and testing sets using various strategies:
        * Normal Train-Test Split: A standard split is applied to different dataframes (`df_reversed_high_correlations`, `selected_df`).
        * Stratified Train-Test Split:  A stratified split is applied to `df_reversed` to maintain class proportions in training and testing sets, especially important for potentially imbalanced data.
    * Model Selection and Training:  Several machine learning models are trained and evaluated:
        * Logistic Regression
        * Decision Tree
        * Support Vector Machine (SVM)
        * K-Nearest Neighbors (KNN)
    * Hyperparameter Tuning:  Optimal hyperparameters for each model are determined, particularly after the stratified train-test split, to maximize model performance.


## Models

The following models are used for income classification:

* Logistic Regression
* Decision Tree
* Support Vector Machine (SVM)
* K-Nearest Neighbors (KNN)

## Evaluation Metrics

Model performance is evaluated using appropriate metrics ( accuracy, precision, recall, F1-score, AUC-ROC).



