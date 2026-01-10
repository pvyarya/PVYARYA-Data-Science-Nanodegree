# PVYARYA-Data-Science-Blog-Post
**Motivation**

The goal of this project is to walk through the CRISP-DM process to build and evaluate a predictive machine learning model, while also effectively communicating findings to an audience in the form of a blog. The project highlights exploratory data analysis, model development, evaluation, and interpretation of results. We aim to build a linear regression machine learning model to predict the GDP growth rate.

**Libraries Used**

This project makes use of the following Python libraries:

pandas – for data manipulation and cleaning

numpy – for numerical operations

matplotlib / seaborn – for visualizations in exploratory data analysis

scikit-learn – for model building, evaluation, and metrics

jupyter notebook – for running and presenting analyses interactively

**Files in This Repository**

README.md - Project overview, methodology, and results (this file)

GDP_GROWTH.csv - Dataset used in the analysis

PVYARYA UNEMPLOYMENT.ipynb - notebook containg Exploratory Data Analysis with visualizations and summary statistics, missing values handling, model training, and evaluation

**CRISP-DM**

•	Business Understanding
  
  •	Objective: Create a model to predict UK GDP growth using macroeconomic features
 
  •	Key Questions:
Can we forecast UK GDP growth using macroeconomic features like inflation, unemployment, lending rates, and consumer prices?
What relationships do we observe between our macroeconomic features and GDP growth rate?
How well can the model handle external shocks?

•	Data Understanding
  
  •	Data Sources: The World Bank Databank
 
  •	Data Exploration: 
Some years show negative GDP growth despite low unemployment, highlighting external shocks like COVID-19 in 2020.
High inflation years coincide with high lending rates, reflecting monetary tightening to control inflation.
Extreme recession events such as in 2009 and 2020 show sharp GDP declines. While macro features explain trends, external shocks can have large effects that the models may not be able to predict; we will observe how well the model handles predicting these shocks
GDP growth reacts with a lag to changes in interest rates or unemployment; to develop the model further, one could benefit from adding lagged variables.

•	Data Preparation
 
  •	Cleaining: ffill() is required as columns values have null values. NB: modelling cannot be done if there are NA values
 
  •	Feature Selection: GDP level was not selected, due to its constant trend upwards; not much value can be derived from this. All other feaures had some value

•	Modeling
 
  •	Used linear regression models

•	Evaluation
Model validated with unseen data to ensure generalisation
  
  •	Metrics: 
Relative errors
RMSE for overall prediction error

•	Deployment
  
  •	Created a good initial model; improvements can be made including other features for modelling (both macro variables and not), a larger data set (through utilising perhaps monthly data set), finding equivalent data with more data points, and using alternative models, such as ARIMAX.


**Summary of Results**
I was able to create a linear regression machine learning model. The model is fairly robust, but there may be underfitting present. However, the low test error suggests using the model will provide useful predictions. A very good intial model iteration is created and can be applied to real-world decision-making.

Please see attached the link to the blog, which summarises the results at a high level: https://medium.com/@pranav.arya.pa/is-it-possible-to-predict-the-growth-rate-of-the-uk-before-results-are-released-48c5c5d80bec

**Acknowledgments** 
To The World Bank Databank for providing the dataset for the project.
