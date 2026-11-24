# Sales Analysis

An exploratory data analysis project that examines customer demographics and purchasing behavior using sales transaction data. The analysis is implemented in [main.ipynb](./main.ipynb) with NumPy, pandas, Matplotlib, and Seaborn.

## Project Overview

The notebook explores the factors associated with sales and purchasing patterns, including:

- Gender
- Age group
- Marital status
- State and zone
- Occupation
- Product category
- Product ID
- Number of orders
- Purchase amount

The main goal is to identify the customer segments and product categories that contribute most to sales.

## Dataset

The source data is stored in [data.csv](./data.csv).

- Initial shape: **11,251 rows and 15 columns**
- Final cleaned shape: **11,239 rows and 13 columns**
- Target sales measure: `Amount`
- Order measure: `Orders`

Key columns include `User_ID`, `Cust_name`, `Gender`, `Age Group`, `Age`, `Marital_Status`, `State`, `Zone`, `Occupation`, `Product_Category`, `Orders`, and `Amount`.

## Data Cleaning

The notebook performs the following cleaning steps:

1. Loads `data.csv` using UTF-8-compatible Unicode escape handling.
2. Removes the blank `Status` and `unnamed1` columns.
3. Checks and drops rows with missing values.
4. Converts `Amount` from a floating-point value to an integer.
5. Uses summary statistics to review the `Age`, `Orders`, and `Amount` columns.

After cleaning, the dataset contains no missing values.

## Exploratory Analysis

### Gender

The analysis compares the number of buyers and total purchase amount by gender.

- Female customers generated approximately **₹74.34 million** in sales.
- Male customers generated approximately **₹31.91 million** in sales.
- Women account for both a larger buyer count and greater purchasing power in the dataset.

### Age

The age-group comparison shows that customers in the **26-35** age group form the largest active buyer segment, especially among women.

### State

Sales and order counts were aggregated by state and the top ten states were visualized.

- Uttar Pradesh
- Maharashtra
- Karnataka

These states have the highest combined order and sales contributions.

### Marital Status

The purchase amount is compared across marital status and gender.

- Married customers represent the largest buyer group.
- Married women show higher purchasing power than the other segments shown in the analysis.

### Occupation

The notebook compares buyer counts and sales across occupations.

The strongest represented occupations are:

- IT sector
- Healthcare
- Aviation

### Product Category

The final category analysis compares the number of products sold and total sales.

The leading categories are:

- Food
- Clothing
- Electronics

The notebook also identifies the top 15 product IDs by total orders.

## Conclusion

The analysis indicates that the most likely high-value customer segment is:

**Married women aged 26-35 from Uttar Pradesh, Maharashtra, or Karnataka, working in IT, Healthcare, or Aviation, who purchase products in the Food, Clothing, and Electronics categories.**

## Tools and Libraries

- Python
- Jupyter Notebook
- NumPy
- pandas
- Matplotlib
- Seaborn

## Getting Started

1. Install the required Python packages:

   ```bash
   pip install numpy pandas matplotlib seaborn jupyter
   ```

2. Start Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

3. Open [main.ipynb](./main.ipynb) and run the cells in order.