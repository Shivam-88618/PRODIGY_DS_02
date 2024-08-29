EDA and Visualization of a Randomly Generated Dataset
This Python program generates a synthetic dataset containing demographic and behavioral information, cleans the data by handling missing values and duplicates, and then performs exploratory data analysis (EDA). The program uses various visualizations to explore the relationships between different variables within the dataset.

Features
Random Data Generation: Generates a dataset with 1000 samples containing the following features:

Age: Integer values between 18 and 69.
Gender: Randomly chosen between 'Male' and 'Female'.
Income: Integer values between 20,000 and 120,000.
Spending_Score: Integer values between 1 and 99.
City: Randomly chosen from a list of five major U.S. cities.
Data Cleaning:

Missing values are introduced randomly in the Income and Spending_Score columns.
Missing values are filled using the median of the respective columns.
Duplicate rows, if any, are removed.
The Gender and City columns are converted to categorical data types for efficient storage and processing.
Exploratory Data Analysis (EDA):

Distribution of Age: Visualized using a histogram with a kernel density estimate (KDE) overlay.
Distribution of Income: Visualized using a histogram with a KDE overlay.
Gender Distribution: Visualized using a count plot.
Relationship between Age and Spending Score: Visualized using a scatter plot, with points colored by gender.
Relationship between Income and Spending Score: Visualized using a scatter plot, with points colored by city.
Dependencies
To run this program, you'll need the following Python libraries:

pandas
numpy
seaborn
matplotlib
You can install these dependencies using pip:

pip install pandas numpy seaborn matplotlib

Usage
Set Up the Environment: Ensure you have Python installed along with the required libraries.

Run the Script: Execute the script to generate the random dataset, clean it, and perform the exploratory data analysis.

python script_name.py

View the Output: The program will display the following visualizations:
Age Distribution: A histogram showing the frequency distribution of ages.
Income Distribution: A histogram showing the frequency distribution of income.
Gender Distribution: A count plot showing the number of samples for each gender.
Age vs. Spending Score: A scatter plot showing the relationship between age and spending score, differentiated by gender.
Income vs. Spending Score: A scatter plot showing the relationship between income and spending score, differentiated by city.
How It Works
Data Generation:

The script generates a dataset with 1000 samples, containing five features: Age, Gender, Income, Spending_Score, and City.
Random missing values are introduced in the Income and Spending_Score columns.
Data Cleaning:

Missing values are handled by filling them with the median value of their respective columns.
The script checks for and removes any duplicate rows.
Categorical variables (Gender and City) are converted to appropriate data types for efficient analysis.
Exploratory Data Analysis:

The script uses seaborn and matplotlib to generate visualizations that help to understand the distribution and relationships between the features.
Customization
Number of Samples: You can modify the n_samples variable to increase or decrease the number of generated samples.
City Choices: You can customize the list of cities from which the City feature is randomly selected.
Data Visualization: The visualizations can be customized by modifying the seaborn and matplotlib plot parameters.
Example Output
Age Distribution
A histogram showing the age distribution among the samples.
Income Distribution
A histogram showing the income distribution among the samples.
Gender Distribution
A count plot displaying the number of male and female samples.
Age vs. Spending Score
A scatter plot showing the relationship between age and spending score, with points colored by gender.
Income vs. Spending Score
A scatter plot showing the relationship between income and spending score, with points colored by city.


Author
This script was created as an educational tool to demonstrate data generation, cleaning, and exploratory data analysis using Python.
