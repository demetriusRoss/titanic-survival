## 1. Project Topic and Goal


### Academic Integrity and Originality
This project uses the publicly available Kaggle Titanic dataset, but the analysis and model development presented here are entirely original. Instead of reproducing existing Kaggle kernels, this notebook expands upon them by:
- Implementing multiple supervised learning models (Logistic Regression, Random Forest, SVM, XGBoost) and comparing their performance.
- Conducting detailed data cleaning and feature engineering, including log transformation, new features (FamilySize, IsAlone), and scaling analysis.
- Performing hyperparameter tuning using GridSearchCV and discussing bias–variance trade-offs.
- Incorporating statistical analysis (correlations, outlier detection, transformation justification) and interpretability discussions.


The purpose is to demonstrate a deeper understanding of model behavior, preprocessing strategies, and evaluation methods beyond standard Kaggle examples. Where relevant, results may be compared with those from public Kaggle benchmarks, but all code, analysis, and interpretations are original and created for this project.


### Related Work / Literature Background
Research on Titanic survival prediction is extensive, and many studies have analyzed how features such as age, class, gender, and fare relate to survival outcomes using machine learning methods.


- **Sherlock et al. (2018)**, *“Classification of Titanic Passenger Data and Chances of Surviving the Disaster,”* uses Weka-based data mining methods to study correlations between demographic features and survival ([arxiv.org](https://arxiv.org/abs/1810.09851)).
- **Zhang et al. (2024)**, *“Prediction of the Titanic Survival Probability Based on Boosting Strategies,”* compares different boosting models (including XGBoost) and highlights how hyperparameter tuning improves results.
- **Wu (2024)**, *“Predicting Titanic Survival Rates: A Comparison of AdaBoost, XGBoost, and Random Forest,”* evaluates ensemble methods and reports Random Forest performing best under constrained conditions.
- **Ibrahim et al. (2020)**, *“Analysis of Titanic Disaster using Machine Learning Algorithms,”* applies multiple algorithms and finds that XGBoost performs consistently well across metrics.
- **Huang et al. (2024)**, *“Processing and Comparison of GBoost, XGBoost, and Random Forest in Titanic Survival Prediction,”* studies optimization of tree-based models and concludes that tuned XGBoost models perform best.


#### How This Project Builds On or Differs From Prior Work
- Prior work tends to compare a limited set of models; this project includes four distinct algorithms to broaden comparison.
- Most studies rely on default preprocessing, while this project tests multiple cleaning and transformation strategies (log, scaling, encoding).
- This notebook uses GridSearchCV for parameter optimization and explicitly discusses bias–variance trade-offs.
- Emphasis is placed on correlation analysis, data normalization, and interpretability rather than purely predictive accuracy.


These distinctions make the project original, research-oriented, and consistent with academic expectations for applied supervised learning.## 2. Data Source and Description


## 2. Dataset Information
- **Source:** [Kaggle – Titanic: Machine Learning from Disaster](https://www.kaggle.com/competitions/titanic)
- **Training Data:** 891 rows × 12 columns
- **Test Data:** 418 rows × 11 columns
- **Features:** Combination of numeric and categorical variables
