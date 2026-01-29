Project Overview:This project focuses on the Feature Engineering phase of the machine learning pipeline. Using the "Adult Income Dataset," I performed data cleaning, categorical encoding, and numerical scaling to prepare the data for predictive modeling.
Tech StackLanguage: PythonLibraries: Pandas (Data Manipulation), Scikit-Learn (Preprocessing)Dataset: Adult Income Dataset (UCI Machine Learning Repository)
Implementation Steps
1. Data IdentificationSeparated features into Categorical (Object) and Numerical (Int/Float) types.Identified "Salary" as the target variable for binary classification.
2.Categorical EncodingLabel Encoding: Applied to the target variable (salary) to convert classes into $0$ and $1$.One-Hot Encoding: Applied to nominal features like race and sex.
Used drop_first=True to eliminate redundant data and avoid the Dummy Variable Trap
3. Feature ScalingMethod: StandardScaler (Standardization).Applied to: age and hours-per-week.Result: Transformed features to have a mean of 0 and a standard deviation of 1.
 This ensures that the model treats all features with equal importance regardless of their original units.
