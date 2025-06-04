# Project Title: Titanic Dataset - Data Cleaning & Exploratory Data Analysis (EDA)

## Problem Definition
The goal of this project is to perform data cleaning and exploratory data analysis (EDA) on the Titanic dataset from Kaggle to uncover patterns and trends, especially factors that influenced survival.

## Dataset
- Source: Kaggle Titanic Competition Dataset
- The dataset contains information such as passenger details, class, fare, age, gender, cabin, ticket number, and survival status.

## Tools & Libraries
- Python
- Pandas for data preprocessing
- Matplotlib and Seaborn for data visualization
- Jupyter Notebook for running the analysis

## Data Collection
- The dataset was loaded using Pandas.
- An initial preview was done to understand the structure and get a glimpse of the records.
- Key features like PassengerId, Name, Sex, Age, Pclass, and Survived were identified as relevant.

## Data Exploration
- Dimensions of the dataset were examined to find the number of rows and columns.
- A list of all column names was reviewed.
- Basic info including data types and null value counts was retrieved.
- Missing values were detected in the `Age`, `Cabin`, and `Embarked` columns.
- Descriptive statistics were used to understand the spread, central tendency, and possible outliers in numeric columns.

## Data Cleaning
- The `Cabin` column was dropped due to excessive missing data.
- Missing values in the `Age` column were filled using the median to reduce the impact of outliers.
- The `Embarked` column was imputed with its mode since it had only a few missing values.
- Categorical columns like `Sex` and `Embarked` were converted to numeric values for easier analysis:
  - `Sex`: male as 0, female as 1
  - `Embarked`: S as 0, C as 1, Q as 2

## Exploratory Data Analysis (EDA)

### Survival Rate
- A count plot was created to show the number of passengers who survived versus those who didn’t.
- This helped understand the class imbalance in survival.

### Survival by Gender
- A bar chart compared survival rates between male and female passengers.
- Females had a noticeably higher survival rate, likely due to evacuation priorities.

### Survival by Passenger Class
- A count plot was used to show how survival varied across passenger classes.
- First-class passengers had higher survival rates, suggesting a correlation between social status and survival chance.

### Age Distribution by Survival
- A histogram was used to visualize the distribution of ages for survivors and non-survivors.
- Young children had better survival rates, while older adults had poorer outcomes.

### Correlation Heatmap
- A heatmap was generated to visualize the correlation between numeric features.
- It revealed that gender and class were significantly correlated with survival.

### Pairplot of Key Features
- A pairplot was created to explore interactions between survival, class, fare, and age.
- It showed that survivors often belonged to lower class numbers (1st class) and paid higher fares.

## Observations
- Survival was influenced strongly by gender, passenger class, and age.
- Females and children had higher survival rates.
- First-class passengers were more likely to survive than those in 2nd or 3rd class.
- These insights can be used for predictive modeling or further machine learning tasks.

