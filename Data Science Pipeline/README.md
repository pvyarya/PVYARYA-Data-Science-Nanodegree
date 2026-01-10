Motivation

The objective is to build a machine learning pipeline that integrates numerical, categorical, and text review data to predict whether a StyleSense customer would recommend a product, enabling automated insights into customer satisfaction and product trends.

Libraries Used

This project makes use of the following Python libraries:

os - For interacting with the operating system

glob - For finding files that match a pattern 

re - For regular expressions, often used to clean review text

joblib - For saving and loading trained models/pipelines efficiently

pathlib.Path - Modern, object-oriented way to handle file system paths.

numpy (np) - Fast numerical operations, arrays, reshaping.

pandas (pd) - Handling tabular data

train_test_split - To split data into train and test sets

GridSearchCV - For hyperparameter tuning with cross-validation

cross_val_score - To evaluate model performance across folds

Pipeline - To chain preprocessing steps + model training into a single workflow

ColumnTransformer - To apply different preprocessing to different feature types

Numerical - imputation + scaling

Categorical - imputation + one-hot encoding

Text - TF-IDF

SimpleImputer - To handle missing values

OneHotEncoder - To encode categorical features into numerical vectors.

StandardScaler - To normalize numerical features

FunctionTransformer - To apply custom transformations

TfidfVectorizer - To turn raw review text into numerical features

LogisticRegression - A strong baseline classification model

RandomForestClassifier - More powerful, non-linear model that handles feature interactions well

accuracy_score, precision_score, recall_score, f1_score → Standard metrics to evaluate classifier performance.

confusion_matrix - To analyze true/false positives/negatives.

classification_report - To summarize precision, recall, F1-score per class.


Files in This Repository

README.md - Project overview, methodology, and results (this file)

reviews.csv - Dataset used in the analysis

nlp_pipeline.ipynb - notebook that is a NLP Model Pipeline.

Summary of Results I was able to create a NLP Pipeline. Using the fine-tuned model against the test set to observe its performance, we observe the accuracy is very high, and it can be used.

Acknowledgments: Code in notebook is adapted from Udacity Data Scientist Nanodegree- Course 4 Data Science Pipelines
