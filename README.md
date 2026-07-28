# Data Science Project 1 – Data Preprocessing for E-Commerce Dataset

## Project Objective

The objective of this project is to clean, transform, and prepare an e-commerce dataset for analysis and machine learning. The project demonstrates the complete data preprocessing workflow, including data exploration, quality assessment, missing value treatment, outlier detection, feature engineering, data validation, and dataset export.


## Dataset

**Dataset Name:** Dataset for Data Analytics.xlsx

The dataset contains customer transaction records from an e-commerce business. Each record includes information such as:

* Order ID
* Order Date
* Customer ID
* Product
* Quantity Purchased
* Unit Price
* Shipping Address
* Payment Method
* Order Status
* Tracking Number
* Items in Cart
* Coupon Code
* Referral Source
* Total Price

### Dataset Summary

* **Rows:** 1,200
* **Original Features:** 14
* **Data Types:** Numerical, Categorical, and Datetime


## Libraries Used

The following Python libraries were used throughout the project:

* pandas
* numpy
* matplotlib
* seaborn
* scikit-learn
* scipy
* openpyxl


## Project Structure

```text
Data Science Project 1/
│
├── dataset/
│      Dataset for Data Analytics.xlsx
│
├── notebooks/
│      Data_Cleaning.ipynb
│
├── outputs/
│      cleaned_dataset.csv
│      cleaned_dataset.xlsx
│      plots/
│
├── report/
│      Data_Preprocessing_Report
│
├── scripts/
│
└── README.md
```


## Steps Performed

### 1. Data Loading

* Imported required libraries
* Loaded the Excel dataset
* Examined dataset dimensions
* Inspected data types
* Previewed the dataset

### 2. Data Exploration

* Generated descriptive statistics
* Identified numerical and categorical variables
* Examined feature distributions
* Computed the correlation matrix
* Created exploratory visualisations

### 3. Data Quality Assessment

* Checked for missing values
* Calculated missing value percentages
* Investigated missing data patterns
* Detected duplicate records
* Verified data types
* Reviewed category consistency

### 4. Missing Value Treatment

* Analysed missing values
* Compared imputation methods
* Replaced missing CouponCode values with **"No Coupon"**
* Confirmed no missing values remained

### 5. Outlier Detection and Treatment

* Detected outliers using the Interquartile Range (IQR) method
* Detected outliers using the Z-score method
* Visualised outliers with boxplots and scatterplots
* Applied IQR-based capping to reduce the influence of extreme values

### 6. Feature Engineering

Created additional variables, including:

* AverageSpendPerCartItem
* OrderMonth
* OrderQuarter
* OrderYear
* WeekendOrder

### 7. Data Encoding

Categorical variables were converted into numerical representations using:

* Label Encoding
* One-Hot Encoding

### 8. Feature Scaling

Numerical variables were standardised using StandardScaler.

### 9. Data Validation

Verified that:

* No missing values remained
* Data types were valid
* Outliers were treated
* Engineered features were successfully created
* The dataset was ready for analysis

### 10. Export

The final processed dataset was exported as:

* cleaned_dataset.csv
* cleaned_dataset.xlsx


## Results

The preprocessing pipeline successfully transformed the raw dataset into a clean, consistent, and analysis-ready dataset.

Key outcomes include:

* Missing values successfully handled
* No duplicate records
* Appropriate data types maintained
* Outliers treated using IQR capping
* Five new engineered features created
* Categorical variables encoded
* Numerical variables scaled
* Clean dataset exported in CSV and Excel formats


## Visualisations Produced

The project includes visualisations comparing the dataset before and after preprocessing, including:

* Missing value heatmaps
* Boxplots
* Histograms
* Correlation heatmaps
* Monthly order distribution
* Quarterly order distribution
* Weekend versus weekday order distribution


## How to Run

### 1. Clone the repository

```bash
git clone <repository-url>
```

### 2. Navigate to the project folder

```bash
cd "Data Science Project 1"
```

### 3. Install the required libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn scipy openpyxl
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

### 5. Open the notebook

Navigate to:

```
notebooks/Data_Cleaning.ipynb
```

Run all cells from top to bottom.

The cleaned datasets will be generated in the `outputs/` directory, while the report and visualisations can be found in their respective folders.


## Author

**Abasifreke Willie**

Data Analyst | Data Science Enthusiast
