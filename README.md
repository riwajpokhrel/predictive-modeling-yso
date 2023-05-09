# predictive-modeling-yso

*A machine learning exercise designed to classify young stellar objects that are detected in the infrared radiation in nearby molecular clouds, and to predict missing values in observation using the trained model.*

The repo contains following files- 

ysoClass_logisticRegression.ipynb: Using Logistic Regression to classify young stellar objects from Gutermuth et al (2009). The technique of Multiple Copula Imputation is used to predict missing values. The algorithm decomposes joint probability distributions into their marginal distributions and a function, the copula, that couples them. Steps for EDA, feature engineering, and feature scaling are explained.

ysoClass_rf.ipynb: Uses CART based Decision Trees to classify young stellar objects in molecular clouds that are <2 kpc away. Excerices on feature engineering and selecting important feature variables. The second part of the code implements the Random Forest algorithm in improving the accuracy of the model. Both DT and RF models are trained with the young stellar object census in Gutermuth et al. (2009). This trained model is used to predict the classification of young stellar objects in the Milky Way galaxy.

ysoClass_impute_test.ipynb: A RF trained model is used to predict the missing values in observation. For test purpose, a certain fraction of observation is first set to NaN (missing). The RF model is trained with the remaining non-nan data. The trained model is used to predict missing values. A comparison between the actual values (before assigning NaN) and predicted values is presented.

table4_Gutermuth09.csv: Table 4 from Gutermuth et al. (2009). It shows classification of infrared sources as deeply embedded (Class 0), protostellar (Class 1), primordial disk (Class 2), and transitional disk (Class 3) candidates. 


References:
- Gutermuth et al. 2009, ApJS, 184, 18
