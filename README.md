# One-Hot-Encoding

**Home Prices Prediction using One-Hot Encoding**
This project demonstrates the use of one-hot encoding to handle categorical variables and predict home prices using linear regression. The dataset includes information about house prices and the towns they are located in.

**Dataset**
The dataset homeprices_one_hot_encoding.csv contains three columns:
**town:** The town where the house is located.
**area:** The area of the house in square feet.
**price:** The price of the house in US dollars.

**Steps**
**Data Loading and Preparation:**
Loaded the dataset into a DataFrame.
Applied one-hot encoding to the town column to convert categorical data into numerical data.
Merged the one-hot encoded columns back into the original DataFrame.
Dropped the original town column and one of the one-hot encoded columns to avoid multicollinearity.

**Model Training:**
Trained a linear regression model using the processed DataFrame.
Separated the features (area and one-hot encoded town columns) and the target (price) for model training.

**Prediction:**
Predicted the price of a house given its area and town.
Evaluated the model's accuracy.

**Alternative Approach:**
Used LabelEncoder and OneHotEncoder from sklearn to handle the categorical variable.
Transformed the town column to numerical labels.
Applied one-hot encoding and removed one of the columns to avoid multicollinearity.
Trained a linear regression model using the transformed data.
Predicted the price of a house given its area and town.

**Dependencies**
pandas
numpy
scikit-learn
