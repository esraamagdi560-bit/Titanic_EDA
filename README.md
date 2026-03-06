# Titanic EDA Project

This project is an **Exploratory Data Analysis (EDA)** of the **Titanic dataset** from Kaggle.  
The goal is to understand patterns and factors affecting passenger survival.

---

## Dataset

- Source: [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic/data)
- Main columns:
  - `Survived` → Survival (0 = No, 1 = Yes)
  - `Pclass` → Passenger Class (1 = 1st, 2 = 2nd, 3 = 3rd)
  - `Sex` → Gender
  - `Age` → Age of passenger
  - `Fare` → Ticket fare
  - `Embarked` → Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

---

## Steps Performed

1. **Data Loading** – Loaded the dataset using `pandas`.
2. **Data Overview** – Checked data types, missing values, and basic statistics.
3. **Data Cleaning** – 
   - Filled missing `Age` values with mean.
   - Dropped unnecessary columns: `Cabin`, `Name`, `Ticket`, `PassengerId`.
4. **Data Encoding** – Converted categorical variables:
   - `Sex` → 0 = Female, 1 = Male
   - `Embarked` → One-hot encoding
5. **Visualization** – Explored key patterns with:
   - Bar plots (Survival by Gender, Class, Age groups)
   - Heatmaps (Correlations, Survival by Class and Gender)
6. **Insights Extraction** – Generated observations from patterns and correlations.

---

## Key Visualizations

- **Overall Survival Count**
- **Survival Rate by Gender**
- **Survival Rate by Passenger Class**
- **Survival Rate by Gender & Class**
- **Age Distribution**
- **Correlation Heatmap**

---

## Insights

1. Only **~38% of passengers survived**; majority (~62%) did not survive.  
2. **Females had a much higher survival rate (~75%)** compared to males (~19%).  
3. **Higher class passengers survived more**:
   - 1st Class: 62% survival
   - 2nd Class: 48% survival
   - 3rd Class: 24% survival
4. Combining **gender and class** shows female 1st-class passengers had the highest survival, while male 3rd-class passengers had the lowest.  
5. **Younger passengers**, especially children, had slightly higher survival chances.  
6. Higher fares correlate with higher survival probability.  
7. **Pclass negatively correlates** and **Fare positively correlates** with survival.

---

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/username/Titanic_EDA.git
