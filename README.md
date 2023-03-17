# Ensemble_modeling
churn prediction i.e to predict whether a driver will be leaving the company or not based on their attributes
Dataset is of
1. MMMM-YY : Reporting Date (Monthly)
2. driver_ID : Unique id for drivers
3. Age : Age of the driver
4. Gender : Gender of the driver – Male : 0, Female: 1
5. City : City Code of the driver
6. Education_Level : Education level – 0 for 10+ ,1 for 12+ ,2 for graduate
7. Income : Monthly average Income of the driver
8. Date Of Joining : Joining date for the driver
9. LastWorkingDate : Last date of working for the driver
10.Joining Designation : Designation of the driver at the time of joining
11.Grade : Grade of the driver at the time of reporting
12.Total Business Value : The total business value acquired by the driver in a month (negative business indicates cancellation/refund or car EMI adjustments)
13.Quarterly Rating : Quarterly rating of the driver: 1,2,3,4,5 (higher is better)

Concepts used
1. Ensemble Learning- Bagging
2. Ensemble Learning- Boosting
3. KNN Imputation of Missing Values
4. Working with an imbalanced dataset

Steps followed.
1. Imported the dataset and did exploratory analysis steps like checking the structure & characteristics of the dataset.
2. Converted date-like features to their respective data type
3. Checked for missing values and Prepared data for KNN Imputation
4. Aggregated data in order to remove multiple occurrences of same driver data 
5. Feature Engineering 
6. Created a column which tells whether the quarterly rating has increased for that driver 
7. Target variable creation: Create a column for target which tells whether the driver has left the company - driver whose last working day is present will have the value 1
8. Created a column which tells whether the monthly income has increased for that driver - for those whose monthly income has increased, assigned the value 1
9. Statistical summary of the derived dataset
10. Checked correlation among independent variables and how they interacted with each other
11. One hot encoding of the categorical variable
12. Class Imbalance Treatment
13. Standardization of training data
14. Used Ensemble learning - Bagging, Boosting methods with some hyper-parameter tuning

Results Evaluation:
Classification Report
ROC AUC curve
Provided actionable Insights & Recommendations
