### SCT_DS_TSK 1
### SCT_DS_TSK 2
### SCT_DS_TSK 3
### SCT_DS_TSK 4

# SCT_DS_TSK 1

# Population Data Visualization: SkillCraft Technology Internship Task 1
## Overview
This project visualizes the distribution of population data for various countries around the world, with a focus on the year 2010. The task involves creating bar charts to visualize the top 10 and bottom 10 countries by total population, as well as exploring gender-specific populations (male and female) in these countries.

## Task Description
Task: Create bar charts or histograms to visualize the distribution of a categorical or continuous variable such as the distribution of ages or gender in population.
Task Completed By: Althaf N.
## Project Structure
The project consists of the following:

Data Cleaning : Importing and cleaning population data.
Visualization:
Bar charts showing the top 10 and bottom 10 countries based on total population in 2010.
Gender-specific population analysis (for male and female populations in 2010).
Python Libraries Used:
pandas: For data manipulation and analysis.
matplotlib: For creating static, interactive, and animated visualizations.
seaborn: For statistical data visualization.
### Data Source
The data used for this project is from the World Bank population dataset, which includes population statistics for countries across various years.

## Steps Involved
### 1. Data Loading
The dataset is loaded using the pandas library from a CSV file, which contains information on population for different countries and years.

### 2. Data Cleaning
Unnecessary columns such as "Country Code" and "Indicator Name" are dropped.
Rows with missing values are removed for consistency.
### 3. Population Data Filtering
The population data for the year 2010 is extracted, and the countries are sorted by total population for that year.

### 4. Data Visualization
Top 10 countries by population: A bar chart is created to show the top 10 countries with the highest total population in 2010.
Bottom 10 countries by population: A separate bar chart visualizes the bottom 10 countries with the lowest total population in 2010.
Gender-Specific Population: Two additional bar charts visualize the top 10 countries by male and female populations in 2010.
### 5. Visualization Customization
Value labels are added to the bars in the charts to provide exact population values, and the layout is adjusted for clarity.

# SCT_DS-TSK 2

# Titanic Dataset - Data Cleaning and Exploratory Data Analysis (EDA)
This repository contains an analysis of the Titanic dataset available on Kaggle. The goal of this project was to perform data cleaning and exploratory data analysis (EDA) to identify patterns and trends in the data that may help predict the survival of passengers aboard the Titanic. This was an internship task as part of SkillCraft Technology's Data Science program.

## Dataset Source
The dataset used in this project is from the Kaggle Titanic competition.

## Steps Taken
### Step 1: Load the Titanic Dataset
The Titanic dataset was loaded into a pandas DataFrame for analysis.

### Step 2: Data Cleaning
The following steps were performed to clean the data:

Missing Values: Missing values were handled by imputing the Age column with the median, filling missing Embarked values with the most frequent embarkation point, and dropping the Cabin column due to excessive missing values.
Data Types: Columns like Survived, Pclass, and Embarked were converted to categorical data types to improve analysis.
### Step 3: Exploratory Data Analysis (EDA)
EDA was conducted to understand the relationships between various features and survival rates:

Summary Statistics: A quick overview of numerical features was generated.
Visualizations: Distributions for key features like Age, Fare, and Survived were visualized. We also explored survival rates by Sex, Pclass, Age, and Embarked.
Correlation Analysis: A correlation matrix was created to identify relationships between numerical features.
### Step 4: Feature Engineering
New features were created to better capture information:

FamilySize: Combined the number of siblings/spouses (SibSp) and parents/children (Parch) to create a new feature.
IsAlone: A binary feature indicating whether a passenger was traveling alone (based on the FamilySize feature).
### Step 5: Feature Importance
A Random Forest Classifier was used to assess the importance of different features in predicting survival. The most important features were identified and ranked.

### Step 6: Conclusion
Based on the data analysis, we can draw several conclusions:

Women had a higher survival rate than men.
First-class passengers had a higher survival rate than those in lower classes.
Younger passengers had a higher chance of survival.
Passengers who embarked at Cherbourg (C) had a higher survival rate than those who embarked at Southampton (S) or Queenstown (Q).


### SCT_DS_TSK 3

# Decision Tree Classifier for Predicting Customer Purchases

This project involves building a Decision Tree Classifier to predict whether a customer will purchase a product or service based on their demographic and behavioral data. The model is trained using the **Bank Marketing Dataset** from the UCI Machine Learning Repository. 

### Dataset

The dataset used for this project is the [Bank Marketing Dataset](https://archive.ics.uci.edu/dataset/222/bank+marketing) from the UCI Machine Learning Repository. It contains data collected from a marketing campaign of a Portuguese banking institution. The goal of the campaign was to predict if a customer would subscribe to a term deposit based on various features like age, job, marital status, education, and past campaign interactions.

- **Data Features**: 
    - `age`: Age of the customer
    - `job`: Type of job (e.g., admin, blue-collar, technician)
    - `marital`: Marital status
    - `education`: Level of education
    - `default`: Whether the customer has credit in default
    - `housing`: Whether the customer has a housing loan
    - `loan`: Whether the customer has a personal loan
    - `contact`: Type of communication used (e.g., cellular, telephone)
    - `month`: Last contact month of the year
    - `day_of_week`: Last contact day of the week
    - `duration`: Duration of the last contact in seconds
    - `campaign`: Number of contacts performed during this campaign
    - `pdays`: Number of days since the client was last contacted from a previous campaign
    - `previous`: Number of contacts performed before this campaign
    - `poutcome`: Outcome of the previous marketing campaign
    - `y`: Whether the client subscribed to a term deposit (`yes` or `no`)

### Objective

The goal is to predict the value of the `y` column, which indicates whether a customer subscribed to a term deposit. This is a binary classification problem with two possible outcomes: `yes` or `no`.

### Steps Involved

1. **Data Preprocessing**:
    - Load and inspect the dataset.
    - Handle missing values (if any).
    - Encode categorical variables into numeric values (using `LabelEncoder`).
    - Split the dataset into training and testing sets.

2. **Modeling**:
    - Train a **Decision Tree Classifier** using the training dataset.
    - Evaluate the model using various metrics such as accuracy, confusion matrix, and classification report.

3. **Visualization**:
    - Visualize the trained Decision Tree using `plot_tree`.
    - Generate a confusion matrix heatmap to visualize performance.
    - Create additional visualizations such as feature importance, ROC curve, and precision-recall curve to further evaluate the model.


## SCT_DS_TSK 4

# Traffic Accident Analysis (Skillcraft Technology Internship Project)

## Project Overview
This project analyzes traffic accidents in the United States based on data from [US Accidents Dataset](https://www.kaggle.com/datasets/sbhatti/us-accidents). The goal is to identify patterns in traffic accidents related to road conditions, weather, and time of day. Additionally, contributing factors such as the presence of traffic signals, stop signs, and junctions are also analyzed.

## Key Analysis
1. **Accidents by Road Condition**: Identifying how road conditions contribute to accidents.
2. **Accidents by Weather Condition**: Understanding the role of weather in traffic accidents.
3. **Accidents by Time of Day**: Analyzing the frequency of accidents by hour of the day and day of the week.
4. **Contributing Factors**: Examining other factors such as traffic signals, road type, and amenities.
5. **Geospatial Analysis**: Mapping accident locations to identify hotspots.

## Data Preprocessing
- Cleaned and formatted columns like `Start_Time`, `End_Time`, `Weather_Condition`, and `Road_Condition`.
- Extracted time-based features such as `Hour` and `Weekday`.
- Handled missing data for key columns.

## Visualizations
- Distribution of accidents based on road conditions, weather conditions, and time of day.
- Heatmaps and correlation matrices to identify relationships between contributing factors.

## Tools and Libraries
- Pandas for data manipulation
- Matplotlib and Seaborn for visualizations
- Geopandas for geospatial analysis
