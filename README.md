# 🛒 Retail Store Data Analysis

## 📅 Date
27 May 2026

## ✅ Work Done
Data Cleaning

---

# 📌 Project Overview.

This project focuses on cleaning a retail store sales dataset using Python and Pandas in Google Colab.  
The dataset contained missing values, datatype inconsistencies, and categorical null values which were cleaned and prepared for further analysis.

---

# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Google Colab

---

# 📂 Data Cleaning Process

## 1️⃣ Handling Missing Values

- Checked null values using:
  
```python
df.isnull().sum()
```

- Filled numerical missing values using median imputation

```python
df['Price Per Unit'].fillna(df['Price Per Unit'].median(), inplace=True)
```

- Filled categorical/boolean missing values using mode imputation

```python
df['Discount Applied'].fillna(df['Discount Applied'].mode()[0], inplace=True)
```

---

## 2️⃣ Handling Duplicate Values

Checked duplicate rows using:

```python
df.duplicated().sum()
```

No duplicate rows were found in the dataset.

---

## 3️⃣ Handling Datatypes

Corrected inappropriate datatypes in columns.

Examples:
- Quantity → converted to integer datatype
- Discount Applied → converted to boolean datatype

---

## 4️⃣ Outlier Analysis

Outliers in the `Total Spent` column were analyzed using:
- Boxplots
- IQR Method

Business understanding was applied before deciding whether to remove outliers.

---

# 📊 Final Result

The dataset was successfully cleaned and prepared for:
- Exploratory Data Analysis (EDA)
- Dashboard Creation
- Data Visualization
- Machine Learning

---

# 🚀 Learning Outcome

Through this project, I learned:
- Real-world data cleaning techniques
- Missing value handling
- Datatype correction
- Duplicate checking
- Business understanding of outliers

