# Laptop Price Prediction

## Objective
The objective of this project is to develop a machine learning model to predict the prices of laptops based on their specifications.

## Preprocessing Steps Used
Preprocessing is a crucial step in machine learning to enhance the performance of the model. Here are the preprocessing steps used in this project:

- **Handling Missing Values and Duplicates:** Checked for missing and duplicated values in the dataset. Fortunately, there were none.
- **Dropping Unnecessary Columns:** Identified and dropped irrelevant columns, such as 'Unnamed: 0'.
- **Cleaning and Converting Data Types:** Cleaned text data in columns like 'Ram' and 'Weight' by removing units ('GB' and 'kg') and converting them to appropriate data types.
- **Feature Engineering:** Extracted relevant information from certain columns, created new features like 'Touchscreen' and 'Ips' based on the 'ScreenResolution' column, extracted processor brand from the 'Cpu' column, created binary features ('HDD' and 'SSD') based on memory types, and categorized operating systems into broader categories.
- **Splitting Data into Training and Testing Sets:** Split the data into training and testing sets using train_test_split() from scikit-learn to evaluate the model's performance on unseen data.

## Selected Models
For this dataset, three models were chosen:

a. **Linear Regression**  
b. **K Nearest Neighbor**  
c. **Decision Tree**

## Models Accuracies
- **Linear Regression:** 80.73%
- **K Nearest Neighbor:** 80.09%
- **Decision Tree:** 84.63%

## Best Model
The Decision Tree model outperformed the other two models. The improvement in accuracy may be attributed to the following reasons:

- **Handling Complex Relationships:** Decision Trees can handle more complex patterns and relationships in the data compared to linear regression. They can capture distinct interactions between different factors better.
- **Data Flexibility:** Decision Trees can work with different types of data without extensive preparation. They divide the data into smaller groups based on different features, allowing them to create clearer boundaries between different outcomes.

Overall, the Decision Tree model's ability to handle complex relationships and diverse data types likely contributed to its superior performance.

<p align="center">-- *The End* --</p>
