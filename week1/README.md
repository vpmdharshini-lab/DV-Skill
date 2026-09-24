# Superstore Sales Data Analysis 📊

## 📌 Project Overview

This project performs **Exploratory Data Analysis (EDA)** on a Superstore sales dataset using Python.

The analysis focuses on understanding **sales, profit, discounts, product categories, and delivery time**. Different charts and statistical techniques are used to identify patterns and relationships in the data.

## 🎯 Objectives

* Analyze sales performance across different categories.
* Analyze profit across product categories.
* Understand the distribution of sales and profit.
* Calculate delivery time using order and shipping dates.
* Study the relationship between discount and profit.
* Find correlations between numerical variables.
* Visualize important patterns using graphs.

## 🛠️ Technologies Used

* **Python**
* **Pandas** – Data manipulation and analysis
* **NumPy** – Numerical operations
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical visualization
* **Google Colab / Jupyter Notebook**

## 📂 Dataset

The project uses a **Superstore sales dataset** containing **10,194 records and 21 original columns**.

Important columns include:

* Order ID
* Order Date
* Ship Date
* Ship Mode
* Customer ID
* Customer Name
* Segment
* Country/Region
* City
* State/Province
* Postal Code
* Region
* Product ID
* Category
* Sub-Category
* Product Name
* Sales
* Quantity
* Discount
* Profit

The dataset contains three main product categories:

* Furniture
* Office Supplies
* Technology

The notebook also creates an additional **Delivery Days** column from the difference between Ship Date and Order Date.

## 🔍 Data Analysis Performed

### 1. Data Loading

The dataset is loaded using Pandas:

```python
df = pd.read_csv("/content/samplesuperstore.csv")
```

### 2. Data Exploration

The project uses:

```python
df.head()
df.info()
df.describe()
```

to understand the dataset structure and numerical statistics.

### 3. Data Preprocessing

The `Order Date` and `Ship Date` columns are converted into datetime format.

```python
df['Order Date'] = pd.to_datetime(df['Order Date'])
df['Ship Date'] = pd.to_datetime(df['Ship Date'])
```

Delivery time is then calculated:

```python
df['Delivery Days'] = (df['Ship Date'] - df['Order Date']).dt.days
```

The dataset was also checked for missing values, and the notebook shows **0 missing values across the columns checked**.

### 4. Sales Analysis

Total sales are calculated for each category.

The notebook obtains:

| Category        |  Total Sales |
| --------------- | -----------: |
| Furniture       | 754,747.7613 |
| Office Supplies | 731,893.3140 |
| Technology      | 839,893.2790 |

Technology has the highest total sales among the three categories in this analysis.

### 5. Data Visualization

The project creates several visualizations:

* Sales by Category
* Sales Distribution
* Profit by Category
* Sales Distribution by Category
* Profit Distribution
* Profit Variation Across Categories
* Impact of Discount on Profit
* Correlation Heatmap

### 6. Discount and Profit Analysis

A scatter plot is used to examine the relationship between:

**Discount → Profit**

```python
sns.scatterplot(
    data=df,
    x="Discount",
    y="Profit"
)
```

### 7. Correlation Analysis

Numerical columns are selected and their correlation is calculated:

```python
numeric_df = df.select_dtypes(include="number")
corr = numeric_df.corr()
```

A heatmap is then created to visualize the correlations.

## 📈 Key Findings

* The dataset contains **10,194 records**.
* There are **21 original columns**.
* The dataset contains three categories: **Furniture, Office Supplies, and Technology**.
* **Technology** has the highest total sales among the categories.
* Delivery days were calculated from the order and shipping dates.
* No missing values were found in the dataset.
* The analysis examines how discounts are related to profit.
* Correlation analysis is used to understand relationships among numerical variables.

## 📁 Project Structure

```text
Superstore-Sales-Analysis/
│
├── task2.ipynb
├── samplesuperstore.csv
└── README.md
```

## ▶️ How to Run

### Using Google Colab

1. Open `task2.ipynb` in Google Colab.
2. Upload `samplesuperstore.csv`.
3. Make sure the dataset path matches the path used in the notebook.
4. Run the cells from top to bottom.

### Using Jupyter Notebook

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn
```

Then open:

```bash
jupyter notebook task2.ipynb
```

## 👩‍💻 Author

**Dharshini.V**

BCA Student

## ⭐ Conclusion

This project demonstrates how Python can be used for **data cleaning, exploratory data analysis, statistical analysis, and visualization**. The analysis provides insights into sales, profit, discounts, categories, and delivery time using the Superstore dataset.

