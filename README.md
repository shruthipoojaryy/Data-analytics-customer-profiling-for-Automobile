# customer-profiling-for-Automobile

The goal of this project is to perform a Customer Segmentation Analysis for an automobile bike company using an RFM (Recency, Frequency, Monetary) model. This approach groups customers based on their past purchasing behavior, helping the company identify which segments to target for improved sales.

### Key Components

1. **Sales Dashboard**: A dashboard created in Tableau provides insights into customer segments. 

2. **Jupyter Notebooks**: If the notebooks don’t load on GitHub, they are available for viewing on nbviewer:
   - [RFM Analysis.ipynb](#)
   - [DQA and Data Cleaning CustomerDemographic.ipynb](#)
   - [DQA and Data Cleaning NewCustomerList.ipynb](#)
   - [DQA and Data Cleaning Transactions.ipynb](#)
   - [DQA and Data Cleaning Customer Address.ipynb](#)

### Analysis Approach

#### 1. Data Quality Assessment and Cleaning
The first step involved preparing the data by assessing its quality and cleaning it. Here's a summary of the findings:

- **CustomerDemographics.xlsx**:
  - Removed irrelevant columns.
  - Handled missing values by dropping records or imputing values.
  - Standardized gender data and created new features for age and age groups.
  - No duplicate records were found.

- **NewCustomerList.xlsx**:
  - Similar cleaning steps as above.
  - No data inconsistencies or duplicates were found.

- **Transaction_data.xlsx**:
  - Converted a date column to the correct format.
  - Handled missing values and created a new 'Profit' column.
  - No inconsistencies or duplicates found.

- **CustomerAddress.xlsx**:
  - Standardized the states column.
  - Addressed missing customer IDs from the demographics table.

#### 2. Exploratory Data Analysis (EDA)
After cleaning, exploratory analysis provided insights like:

- **Age Distribution**: Most new and old customers are aged 40-49, with fewer customers under 20 or over 80.
- **Purchases by Gender**: Slightly more bikes are bought by females than males.
- **Job Industry Distribution**: New customers mostly come from manufacturing and financial services.
- **Wealth Segmentation**: Most customers are in the 'Mass Customer' segment, with affluent customers growing in the 40-49 age group.
- **Car Ownership by State**: New South Wales has many non-car owners, while Queensland has more car owners.

#### 3. RFM Analysis and Customer Segmentation
Customers were segmented into 11 groups based on RFM analysis:
- **Platinum Customers**
- **Very Loyal Customers**
- **Recent Customers**
- **Potential Customers**
- **Lost Customers**
- **Losing Customers**
- **Late Bloomers**
- **High Risk Customers**
- **Evasive Customers**
- **Becoming Loyal**
- **Almost Lost Customers**

#### 4. Visual Insights
- **Recency vs. Monetary**: Recent customers tend to spend more.
- **Frequency vs. Monetary**: Platinum and loyal customers purchase frequently and contribute more revenue.

### Datasets Used
- **Raw_data.xlsx**: Contains various data sheets.
- **Transactions_data.xlsx**: Customer transaction data.
- **NewCustomerList.xlsx**: Information on new customers.
- **CustomerDemographic.xlsx**: Customer demographic details.
- **CustomerAddress.xlsx**: Customer addresses.

### Tools and Technologies
- **Python**: Used for data quality assessment, cleaning, and exploratory data analysis using libraries like Pandas, Matplotlib, and Seaborn.
- **Tableau**: Used for visualizations and creating the sales dashboard.

