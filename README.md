# Titanic-dataset-Insights
# Titanic Dataset - Superb EDA Report

This project performs a deep Exploratory Data Analysis (EDA) on the famous Titanic dataset using Python and popular libraries like pandas, seaborn, and matplotlib. The goal is to uncover key patterns, trends, and insights from the data through a variety of visualizations and summary statistics.

---

## 📌 Dataset

- **Source**: Titanic dataset (CSV file)
- **Shape**: 891 rows × 12 columns
- **Columns include**: PassengerId, Survived, Pclass, Name, Sex, Age, SibSp, Parch, Ticket, Fare, Cabin, Embarked

---

## 🧪 EDA Steps Performed

### 1. Data Loading and Overview
- Loaded the dataset using `pandas`
- Displayed shape, column names, data types, and summary statistics

### 2. Missing Value Handling
- Filled missing values in `age` with median
- Filled missing `embarked` values with mode
- Dropped `deck` column due to too many missing values

### 3. Data Cleaning
- Removed duplicate rows
- Converted categorical columns to category type

### 4. Univariate Analysis
- Age distribution plotted using **violin plot**
- Fare distribution shown with **histogram + KDE**
- Gender distribution visualized with a **pie chart**

### 5. Bivariate Analysis
- **Survival by gender** using a barplot
- **Fare by class** using swarmplot
- **Age by survival** using violinplot
- **Age vs fare** scatterplot with survival hue

### 6. Outlier Detection
- Detected fare outliers using IQR method

### 7. Correlation Analysis
- Visualized correlation between numeric columns using heatmap

### 8. Feature Engineering
- Added `is_child` feature for passengers under 12
- Created `family_size` as sum of `sibsp` + `parch` + 1

---

## 📊 Key Insights

- Most passengers were aged between 20–40
- Females had a much higher survival rate than males
- First-class passengers had better survival outcomes
- Large families and children showed interesting survival patterns
- Fare had significant outliers and was correlated with class

---

## 🛠️ Tools Used

- Python
- pandas
- seaborn
- matplotlib

---

## ✅ How to Run

1. Install required libraries:
   ```bash
   pip install pandas seaborn matplotlib
