# Graduate-Admission-Prediction
This repository contains a Python script that analyzes admission data using various data visualization techniques and predictive models. The script utilizes the following libraries: pandas, numpy, matplotlib, seaborn, and scikit-learn.

# Dataset
The dataset used in this analysis is stored in the file "Admission_Predict.csv". It contains information about different factors that may influence the chance of admission to a university. The dataset includes the following columns:

-GRE Score
-TOEFL Score
-University Rating
-SOP (Statement of Purpose)
-LOR (Letter of Recommendation)
-CGPA (Cumulative Grade Point Average)
-Research
-Chance of Admit
-Data Analysis
-The script performs the following analysis and visualization tasks:

Load the dataset using pandas and display the first few rows to get an overview of the data.
Remove the "Serial No." column as it does not provide any relevant information.
Print the information about the dataset, including the data types and non-null count of each column.
Generate descriptive statistics for the dataset, including count, mean, standard deviation, minimum, 25th percentile, median, 75th percentile, and maximum values for each numeric column.
Create a correlation heatmap to visualize the relationships between different features.
Perform analysis and visualization on individual features:
Generate descriptive statistics and plot the probability distribution for the GRE scores.
Calculate the correlation coefficients of the GRE scores with other features and display them in a table.
Generate descriptive statistics and plot the probability distribution for the TOEFL scores.
Calculate the correlation coefficients of the TOEFL scores with other features and display them in a table.
Generate descriptive statistics and plot the probability distribution for the CGPA.
Analyze the distribution of research experience among the applicants using a pie chart.
Analyze the distribution of university ratings using a bar chart.
Analyze the distribution of statement of purpose (SOP) ratings using a bar chart.
Analyze the distribution of letter of recommendation (LOR) ratings using a bar chart.
Plot the probability distribution of the chance of admission.
Calculate the descriptive statistics for the chance of admission column.
Calculate the correlation coefficients of the chance of admission with other features and display them in a table.
Prepare the data for modeling:
Separate the features (X) and the target variable (y).
Perform feature scaling using the StandardScaler on the CGPA, GRE Score, and TOEFL Score columns.
Split the data into training and testing sets using train_test_split.
Perform prediction using a linear regression model:
Create a LinearRegression object and fit the model using the training data.
Make predictions on the testing data and calculate the R-squared score, mean squared error, and root mean squared error.
Plot the residuals and the scatter plot of the predicted values against the actual values.
Perform prediction using a decision tree classifier:
Prepare the data for classification by converting the chance of admission into binary labels (0 or 1) based on a threshold.
Split the data into training and testing sets using train_test_split.
Create a DecisionTreeClassifier object and fit the model using the training data.
Make predictions on the testing data and calculate the accuracy, precision, recall, and F1 score.
Visualize the confusion matrix for the testing data.
Visualize the confusion matrix for the training data.
Usage
Install the required dependencies by running pip install pandas numpy matplotlib seaborn scikit-learn in your Python environment.
Download the "Admission_Predict.csv" file and place it in the same directory as the script.
Open the script in a Python IDE or text editor and run it.
The script will generate various plots and display the analysis results in the console.
Note: The script uses deprecated functions distplot and barplot from the seaborn library, which may generate warnings. Consider updating the code to use the recommended functions (displot and histplot) to avoid the warnings.

License
This project is licensed under the MIT License. Feel free to use and modify the code according to your needs.
