# Customers_Data
# Customer Dataset Preprocessing and EDA

## 📌 Project Objective
To explore and clean a customer dataset containing 100,000 entries in preparation for building a predictive model for customer spending behavior.

---

## 📂 Dataset Overview

- **File Name**: `customers_100000.csv`
- **Total Rows**: 100,000
- **Main Columns**:
  - `Customer Id`, `First Name`, `Last Name`
  - `Company`, `City`, `Country`
  - `Phone 1`, `Phone 2`, `Email`, `Website`
  - `Subscription Date`
  - `Amount` (target variable for future prediction)

---

## 🧹 Data Cleaning Steps

1. **Dropped Unnecessary Columns**
   - `hello` and `hello1`: Contained 100% missing values.

2. **Handled Missing Values**
   - `Amount`: Filled missing values using the column's mean.

3. **Removed Duplicates**
   - Ensured unique entries remained in the dataset.

4. **Verified Column Types**
   - Ensured proper types: numeric, object (string), and date-related fields.

---

## 📊 Exploratory Data Analysis (EDA)

- Used `df.describe()` to understand distribution and statistics of numerical fields.
- Checked value counts for key categorical variables like `Country` and `City`.
- Plotted distribution of the `Amount` column using `seaborn.histplot`:
  - Distribution showed skewed spending behavior with a long tail.

---

## ✅ Current Status
The dataset has been:
- Cleaned
- De-duplicated
- Analyzed for basic patterns
- Visualized for key variables

The dataset is now ready for:
- Feature Engineering
- Encoding categorical variables
- Building predictive models

---

## 📁 Next Steps
- Apply one-hot encoding or label encoding for categorical features.
- Select important features for modeling.
- Train a regression model to predict `Amount`.

