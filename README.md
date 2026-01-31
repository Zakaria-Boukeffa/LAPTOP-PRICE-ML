# Laptop Price Analysis and Modeling

## Project Overview

This project aims to apply data science pricnipals in order to analyze laptop prices. 

The project combines **data preprocessing, statistical analysis, unsupervised learning, and supervised learning**.

Prices in the dataset are expressed in Indian Rupees (INR).

---

## Methodology

The project was structured into four main steps.

### 1. Data Preprocessing

The raw dataset required substantial cleaning and transformation:

- Removal of unreliable or highly incomplete variables.
- Extraction of RAM and storage information from unstructured product names
- Standardization of categorical variables.
- Handling of missing values using median imputation
- Normalization of numerical features for modeling purposes

This step was essential, as the data was not clean and contained inconsistencies typical of real-world datasets.

---

### 2. Exploratory Data Analysis (EDA)

The exploratory data analysis was divided into two main stages:

1. **Univariate Analysis**

This step focused on analyzing variables individually:

- Quantitative analysis of numerical features (prices, RAM, storage, savings)

- Qualitative analysis of categorical features (brand, processor type)

2. **Multivariate Analysis**

This stage examined relationships between multiple variables:

- Analysis of relationships between numerical variables

- Comparison of prices across brands and processor types

---

### 3. Modeling

Modeling was divided into two parts.

#### 3.1 Unsupervised Learning

K-Means clustering was applied to normalized quantitative features to identify natural market segments.

Using the Elbow Method, four clusters were selected, corresponding to:
- Entry-level laptops
- Mid-range laptops with balanced specifications
- High-performance laptops
- Premium or gaming laptops

---

#### 3.2 Supervised Learning

Two supervised learning tasks were addressed:

**Price prediction (regression):**
- A linear regression model was used to predict laptop prices
- The model achieved a moderate R² score, showing that hardware specifications explain a significant part of the price variability, but not all of it

**Price classification:**
- Laptop prices were grouped into three categories (Cheap, Average, Expensive) using K-Means
- Several classification models were evaluated
- Logistic Regression achieved the best performance, with accuracy above 80%
- More complex models did not significantly outperform simpler ones
- Naive Bayes performed poorly due to its independence assumption, which is violated by correlated hardware features

---

## Challenges and Limitations

- The dataset required extensive preprocessing due to missing values and unstructured information
- Price distributions contained strong outliers, impacting regression performance
- Some features were highly correlated, limiting the effectiveness of certain models

Despite these challenges, the overall results remained consistent and interpretable.

---

## Conclusion

This project demonstrates how data engineering, exploratory analysis, and machine learning can be combined to study real-world pricing behavior.  

I hope you find this project useful. If you have any suggestions or feedback, please do not hesitate to share them.
