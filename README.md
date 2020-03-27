## Delinquency-prediction  

### Definition: 
 * Delinquency is a condition that arises when an activity or situation does not occur at its scheduled (or expected) date i.e., it occurs    later than expected.  
 * For the given dataset,a consumer is believed to be delinquent if he deviates from the path of paying back the loaned amount within 5      days.  

### Description of Dataset  
 * The dataset consists of **209593 rows** and **37 columns**
 * The decsription of features can be found in the Data_Description file.
 * Quick data exploration was done to find what different data types were present. 
 * **No** missing data was found.
 
### Bi-variate EDA  
 * A bit of bivariate visualization was done to find any correlations
 * Finally, it was seen how much the given features correlated with the target feature('_label_')  
 
### Feature Engineering and Selection  
 * No missing data was found therefore,  there wasn't any need for feature engineering.
 * Collinear features were removed from the dataframe as this helps in generalizing and improving the interpretability of the model.  
 
### Building a predictive model
 * The given data was split into train and test data.
 * Feature scaling was done on X_train and X_test.
 * The models chosen for predicting were:
   1. Random Forest Classifier
   2. Logistic Regression
 * K-Fold cross-validation was done to find best model of the two  
 * Model tuning was done using GridSearchCV
 * Accuracy obtained was **87.7%**
