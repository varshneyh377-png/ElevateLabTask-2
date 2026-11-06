# ElevateLabTask-2
Exploratory Data Analysis

# Titanic Dataset – Exploratory Data Analysis (EDA)

## 📌 Project Overview

This project focuses on performing **Exploratory Data Analysis (EDA)** on the Titanic dataset to understand passenger information and identify the factors that influenced passenger survival during the Titanic disaster.

The main objective is to explore the dataset, clean missing values, identify patterns and outliers, and analyze relationships between different passenger attributes and survival rates using data visualization and statistical techniques.

## 🎯 Objectives

- Understand the structure and characteristics of the Titanic dataset.
- Perform data inspection and cleaning.
- Handle missing values.
- Conduct univariate and multivariate analysis.
- Identify outliers and analyze data distributions.
- Explore relationships between passenger features and survival.
- Perform feature engineering and categorical encoding.
- Understand the important factors associated with passenger survival.

## 📂 Dataset Description

The Titanic dataset contains information about passengers aboard the Titanic.

The dataset consists of **891 rows and 12 columns**.

| Column | Description |
|---|---|
| PassengerId | Unique passenger ID |
| Survived | Survival status (0 = No, 1 = Yes) |
| Pclass | Passenger class (1st, 2nd, 3rd) |
| Name | Passenger name |
| Sex | Gender of passenger |
| Age | Age of passenger |
| SibSp | Number of siblings/spouses aboard |
| Parch | Number of parents/children aboard |
| Ticket | Ticket number |
| Fare | Ticket fare |
| Cabin | Cabin number |
| Embarked | Port of embarkation |

## 🛠️ Technologies & Libraries Used

- **Python** – Programming language
- **Pandas** – Data manipulation and analysis
- **NumPy** – Numerical operations
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical data visualization
- **Scikit-learn** – Handling missing values using SimpleImputer

## 🔍 Project Workflow

### 1. Data Loading and Inspection
- Imported the required Python libraries.
- Loaded the Titanic dataset.
- Examined the dataset using `head()`, `shape`, `columns`, `dtypes`, and `info()`.
- Used `describe()` to understand the statistical properties of numerical features.

### 2. Data Cleaning and Preprocessing
- Removed the Cabin column during preprocessing.
- Handled missing Age values using mean imputation with `SimpleImputer`.
- Filled missing Embarked values using the mode.

### 3. Univariate Analysis

Analyzed individual variables to understand their distributions and characteristics.

The analysis included:
- Survival distribution.
- Passenger class distribution.
- Gender distribution.
- Embarkation port distribution.
- Number of siblings/spouses and parents/children.
- Age distribution using histograms and KDE plots.
- Fare distribution using histograms and box plots.
- Skewness and kurtosis analysis.

### 4. Multivariate Analysis

Explored relationships between multiple variables, particularly their relationship with survival.

The analysis included:
- Survival rate based on passenger class.
- Survival rate based on gender.
- Survival rate based on embarkation port.
- Age distribution among survivors and non-survivors.
- Fare distribution among survivors and non-survivors.
- Pairplot visualization to examine relationships between numerical features.

### 5. Feature Engineering

Created new features to better understand passenger family information.

- Created `Family_size` by combining `SibSp` and `Parch`.
- Categorized passengers into three family types:
  - Alone
  - Medium
  - Large
- Analyzed the relationship between family type and survival.
- Removed the original `SibSp`, `Parch`, and `Family_size` columns after creating the family category.

### 6. Outlier Treatment

- Identified and filtered Age outliers using the three-standard-deviation method.
- Detected Fare outliers using the Interquartile Range (IQR) method.
- Visualized the Fare distribution after outlier treatment.

### 7. Encoding and Correlation Analysis

- Applied one-hot encoding to categorical variables using `pd.get_dummies()`.
- Used `drop_first=True` to avoid redundant dummy variables.
- Generated a correlation heatmap to examine relationships among numerical features.

## 📊 Key Areas of Analysis

The project investigates the following questions:

1. What percentage of passengers survived?
2. How was the passenger population distributed across different classes?
3. Did survival rates differ between male and female passengers?
4. How did passenger class affect survival?
5. Was survival associated with the port of embarkation?
6. How did age and fare distributions differ between survivors and non-survivors?
7. Did family size have a relationship with passenger survival?
8. What patterns and outliers can be identified in the dataset?

## 📈 Visualizations

The project uses Matplotlib and Seaborn to explore the Titanic dataset through different visualizations.

Some of the visualizations include:

- Count plots for survival, passenger class, gender, and embarkation port.
- Histograms and KDE plots for Age and Fare distributions.
- Box plots to examine data distributions and potential outliers.
- Survival comparisons across passenger class, gender, and embarkation port.
- Age and Fare distribution comparisons between survivors and non-survivors.
- Pairplot to explore relationships between numerical features.
- Family type vs. survival visualization.
- Correlation heatmap to examine relationships between features.
  
  <img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/b17afd7a-571a-4612-8154-3d923b430f15" />
  <img width="600" height="500" alt="image" src="https://github.com/user-attachments/assets/1d2cbf18-b5ad-413d-acdd-6287e49d6e8b" />



## 💡 Conclusion

This project demonstrates the process of performing Exploratory Data Analysis on a real-world dataset.

Through data cleaning, statistical analysis, visualization, feature engineering, and correlation analysis, the project explores the relationship between passenger characteristics and survival.

The analysis provides a better understanding of the Titanic dataset and demonstrates how EDA can help uncover meaningful patterns before building machine learning models.

## 🚀 How to Run the Project

1. Clone this repository:

   ```bash
   git clone <your-repository-url>
   ```

2. Navigate to the project directory:

   ```bash
   cd <repository-name>
   ```

3. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```

4. Open the Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Run the notebook cells sequentially.

## 👩‍💻 Project Type

**Exploratory Data Analysis (EDA) | Data Analytics | Python**

---

*This project was completed as a hands-on exercise to strengthen practical skills in data analysis, data visualization, preprocessing, and feature engineering.*
