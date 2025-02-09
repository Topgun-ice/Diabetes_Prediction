# Diabetes_Prediction

## Table of Content
- Description
Importing Libraries
Reading CSV File
Data Cleaning	
Handling Missing Value
Renaming Columns
Filtering rows based on BMI and Smoking History
Sorting Dataset based on Age
Plotting Graph

## Description
This project is set to predict individuals who are liable to getting diabetes and how it occurs based on certain factors or symptoms associated with a diabetic patient. With key details on how certain symptoms like high glucose levels and smoking can influence the risk of having diabetes, detailed graphs explain it all.  

## Importing Libraries
For this project, some libraries were imported including Matplotlib, Pandas and Seaborn for data cleaning and data visualization.

## Reading CSV File
In this project a Comma-Separated Values (CSV) file was used and the pandas library was used to read the dataset of the csv file.

## Data Cleaning
## Handling Missing Values: 
This was done using the fillna() and astype() functions in python. The ‘age’ column is checked for missing values using the fillna() function and the astype() function was used to change the values of the ‘age’ column from a float to an integer. Further data cleaning function was used to generate ages greater-than or equal to 1.

## Renaming Columns: 
The rename() function was used to rename the ‘bmi’ columns to ‘BMI’ for a more professional dataset.

## Filtering rows based on BMI and Smoking History:
The filtering of rows was done using the isin() function to filter out non-smokers since they have lesser chances of having diabetes. Having a BMI ranging from 25.00 to 80.00 is a key indicator of symptoms of diabetes and hence individuals with BMI less than 25.00 were filtered out.

## Sorting Dataset based on Age:
The new dataset was sorted using the values in the ‘age’ column for a clearer and understanding dataset. 

## Plotting Graphs
## Graph 1: Probability of a person getting Diabetes 
Type of Graph: A count plot (bar chart) that displays the number of individuals in your dataset classified as diabetic versus non-diabetic.
Details of the graph:
We use the ‘diabetes’ column (which we defined based on thresholds such as HbA1c ≥ 6.5% or blood glucose level ≥ 126 mg/dL) as the x-axis.
The y-axis shows the frequency (or count) of individuals in each category.
Overview:
This graph illustrates the overall distribution of diabetes in our dataset. The x-axis represents diabetes status with two categories—‘Non-Diabetic’ and ‘Diabetic’—and the y-axis shows the number of individuals in each group.
Key Observations:
For example, if we see that 75% of our sample is non-diabetic and 25% is diabetic, this gives us a clear view of how prevalent diabetes is in my study group.
Implications:
Understanding the prevalence is important as it sets the context for further analysis. If our dataset shows a high prevalence of diabetes, we might need to explore further what factors contribute to this rate, such as lifestyle, genetics, or environmental influences.

## Graph 2: Influence of Blood Glucose Levels on Diabetes
Type of Graph: A Kernel Density Estimate (KDE) plot (or optionally a box plot) comparing the distribution of blood glucose levels for diabetic versus non-diabetic individuals.
Details of the graph:
The KDE plot provides a smooth estimate of the distribution of blood glucose levels, with one curve for non-diabetic individuals and another for diabetic individuals.
Alternatively, a box plot would display the median, quartiles, and potential outliers for each group.
Overview:
This graph compares blood glucose levels between individuals who are diabetic and those who are not. It helps us see if there is a clear difference in the glucose levels of these two groups.
Key Observations:
In the KDE plot, if the curve for diabetic individuals is noticeably shifted to the right (toward higher blood glucose values) compared to the non-diabetic group, it confirms that higher blood glucose levels are associated with diabetes. In the box plot version, we would expect to see a higher median and interquartile range for the diabetic group.
Implications:
These differences support the role of blood glucose as a key marker for diabetes. They also help validate our threshold values for classifying someone as diabetic. For instance, a significant gap between the groups reinforces that a blood glucose level above 126 mg/dL is a strong indicator of diabetes.

## Graph 3: Influence of HbA1c on Diabetes
Type of Graph: A box plot or KDE plot that compares HbA1c levels in diabetic and non-diabetic individuals.
Details of the graph:
With a box plot, you see the median HbA1c levels, the spread of values (the interquartile range), and any outliers for each group.
A KDE plot provides a smooth density estimate of HbA1c levels for both groups.
Overview:
This graph shows how HbA1c levels, which indicate average blood sugar over the past 2–3 months, differ between diabetic and non-diabetic individuals.
Key Observations:
We typically expect the diabetic group to have higher HbA1c values. If using a box plot, the median HbA1c for diabetics should be above the 6.5% threshold, with less overlap between the two groups. In a KDE plot, the density for diabetics should peak at a higher HbA1c value compared to non-diabetics.
Implications:
A clear separation between the two distributions confirms that HbA1c is a reliable diagnostic indicator for diabetes. It also validates our criteria for identifying diabetic individuals in the dataset.

## Graph 4: Gender Distribution Among Diabetic Patients
Type of Graph: A grouped count plot (bar chart) that shows the number of diabetic and non-diabetic individuals within each gender category.
Details of the graph:
The x-axis represents the different gender categories (e.g., Male, Female).
Bars within each gender category are split (using color/hue) by diabetes status.
The height of each bar indicates the count of individuals in that group.
Overview:
This graph breaks down diabetes prevalence by gender, showing the count of diabetic versus non-diabetic individuals for each gender.
Key Observations:
For instance, if we observe that one gender, say males, has a higher count of diabetic individuals than females, it may suggest that men are at a higher risk in our dataset. Conversely, if females show a higher proportion of diabetes, that is equally informative.
Implications:
Understanding gender differences in diabetes prevalence can help target prevention and intervention strategies. It might also prompt further investigation into whether gender-specific factors (such as hormonal differences, lifestyle, or socioeconomic factors) contribute to the risk of developing diabetes.

