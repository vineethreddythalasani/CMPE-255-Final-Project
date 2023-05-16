# CMPE-257-Final-Project
The project involves analyzing Kickstarter campaign data to predict the success of future campaigns. Techniques such as data cleaning, exploratory data analysis, feature engineering, and machine learning models are utilized to create a predictive model.

The given dataset consists of 20,632 Kickstarter campaigns that were analyzed to identify factors contributing to a campaign's success. Here is a summary of the data cleaning and preprocessing steps applied to the dataset:

1. Removing Duplicates: Duplicate campaigns were identified based on the unique campaign ID and removed, resulting in a dataset with 20,632 unique campaigns.

2. Dropping Columns: Several columns with a high number of missing values and potentially limited usefulness for analysis were dropped. These columns included "Unnamed," "Friends," "is_starred," "is_backing," and "permissions."

3. Handling Missing Values: Various columns in the dataset had missing values. For example, the "category" column had a small percentage of missing values, which were imputed using the mode of the column. However, the "location" column had a high percentage of missing values and was dropped entirely.

4. Data Transformation: Certain columns required transformation for consistent analysis. For instance, the "goal" and "pledged" columns were transformed to the same currency (USD), and date columns were converted into datetime objects for time-related analysis.

5. Dimensionality Reduction: To reduce dimensionality and prevent multicollinearity, highly correlated variables were removed from the dataset. Columns with correlation coefficients above 0.7 were dropped to eliminate redundancy and improve model stability.

6. Handling Imbalance Using Upsampling & Downsampling: As the dataset had class imbalance, both upsampling and downsampling techniques were employed. Upsampling involved randomly duplicating samples from the minority class, while downsampling involved randomly removing samples from the majority class. These techniques aimed to balance the representation of both classes in the dataset.

7. Scaling: Feature scaling was performed using the StandardScaler from the sklearn.preprocessing module. Standardizing the range of features ensured that they had similar scales, which is crucial for many machine learning algorithms.

After the data cleaning and preprocessing steps, various models were selected and evaluated for predicting the project state. Logistic Regression, Decision Trees, Random Forest, and SVM were trained and tested on the dataset. Among these models, Decision Trees performed the best with an accuracy of 0.9923. Logistic Regression achieved an accuracy of 0.8913, Random Forest achieved an accuracy of 0.9829, and SVM achieved an accuracy of 0.8927.

Flowchart of Methodologies
![image](https://github.com/vineethreddythalasani/CMPE-257-Final-Project/assets/70748428/2893ed86-8783-4667-8041-793ce15c9cb9)


