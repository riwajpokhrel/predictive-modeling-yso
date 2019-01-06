# predictive-modeling-yso
A machine learning exercise designed to classify young stellar objects that are detected in the infrared radiation in nearby molecular clouds, and to predict missing values in observation using the trained model.

The repo contains following files- 

ysoClass_rf.ipynb: Shows how to make and use decision trees based on CART algorithm, and use such trees to estimate feature importance and predict outcomes in new set of data. This is followed by importance of Random Forest and how it aids in improving the accuracy. The Random Forest model is trained in the young stellar sources presented in Gutermuth et al. (2009). This trained model is used to predict the classification of young stellar objects in other clouds.

ysoClass_impute_test.ipynb: A RF trained model is used to predict the missing values in observation. For test purpose, a certain fraction of observation is first set to NaN and prediction is made on those values based on the model. 

table4_Gutermuth09.csv: Table 4 from Gutermuth et al. (2009). It shows classification of infrared sources as deeply embedded (Class 0), protostellar (Class 1), primordial disk (Class 2), and transitional disk (Class 3) candidates. 


References:
- Gutermuth et al. 2009, ApJS, 184, 18
