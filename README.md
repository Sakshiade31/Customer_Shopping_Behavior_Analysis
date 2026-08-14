# Customer_Shopping_Behavior_Analysis
Data Analytics project includes customer behavior analysis using python, sql and Power BI

**The project includes:**

* Loading and exploring the dataset using Python
* Performing Exploratory Data Analysis (EDA)
* Cleaning and preprocessing the data
* Running SQL queries using PostgreSQL/MySQL
* Creating an interactive Power BI dashboard
* Analyzing the results and generating business insights

## Dataset

The dataset contains structured business/customer data used to perform analysis and identify useful patterns and trends.

The dataset was:

* Loaded into Python using Pandas
* Checked for missing values and duplicates
* Cleaned and transformed for analysis
* Loaded into PostgreSQL/MySQL for SQL analysis
* Used as the source for the Power BI dashboard

## Tools & Technologies

* **Python** – Data loading, cleaning and EDA
* **Pandas** – Data manipulation
* **NumPy** – Numerical operations
* **PostgreSQL / MySQL** – SQL analysis
* **Power BI** – Interactive dashboard and visualization
* **Jupyter Notebook** – Python analysis environment

## Project Steps

### 1. Data Loading

The dataset was imported into Python using Pandas.

```python
import pandas as pd

df = pd.read_csv("dataset.csv")
```

### 2. Exploratory Data Analysis

EDA was performed to understand the structure and quality of the data.

Key activities:

* Checking dataset shape
* Understanding data types
* Checking missing values
* Identifying duplicate records
* Generating statistical summaries
* Analyzing important columns
* Creating visualizations to identify patterns

### 3. Data Cleaning

The dataset was cleaned before performing further analysis.

Steps included:

* Handling missing values
* Removing duplicate records
* Correcting data types
* Renaming columns
* Handling inconsistent values
* Creating useful derived columns/features

### 4. SQL Analysis

The cleaned dataset was imported into **PostgreSQL/MySQL**.

SQL queries were used to perform analysis such as:

* Aggregations
* Filtering and sorting
* GROUP BY and HAVING
* JOIN operations
* Subqueries
* Finding trends and key business metrics

Example:

```sql
SELECT category,
       COUNT(*) AS total_orders,
       SUM(purchase_amount) AS total_sales
FROM orders
GROUP BY category
ORDER BY total_sales DESC;
```

### 5. Power BI Dashboard

The cleaned data was connected to Power BI to create an interactive dashboard.

The dashboard includes:

* KPI cards
* Charts and graphs
* Category-wise analysis
* Trend analysis
* Filters and slicers
* Interactive visualizations

## Dashboard

The Power BI dashboard provides a visual overview of the dataset and helps users quickly understand important business metrics and trends.

**Dashboard Preview:**
<img width="1237" height="737" alt="image" src="https://github.com/user-attachments/assets/f760b2da-4451-479e-9ebe-b20f3196110e" />





## Results & Insights

The analysis helped identify important patterns and trends in the dataset.

Key outcomes:

* Identified important categories and segments
* Analyzed overall sales/performance trends
* Compared different groups using SQL
* Identified patterns through EDA
* Presented key findings through an interactive Power BI dashboard

## How to Run

### Python Analysis

1. Clone the repository.

```bash
git clone <repository-url>
```

2. Navigate to the project directory.

```bash
cd customer_shopping_behavior_analysis
```

3. Install the required Python libraries.

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

4. Open the Jupyter Notebook.

```bash
jupyter notebook
```

5. Open the `.ipynb` file and run the cells sequentially.

### SQL Analysis

1. Install PostgreSQL or MySQL.
2. Create a database.
3. Import the cleaned dataset.
4. Run the SQL queries provided in the `sql` folder.

### Power BI

1. Open the `.pbix` file in Power BI Desktop.
2. If required, update the data source connection.
3. Refresh the data.
4. Explore the dashboard using the available filters and slicers.

