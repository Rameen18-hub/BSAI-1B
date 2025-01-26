# **Data Preprocessing Notebook**
This notebook provides a step-by-step workflow for preprocessing a dataset (apple_sales_2024.csv) using the pandas library. It includes operations such as data exploration, cleaning, and visualization.

# **Key Functions and Operations**
Importing Libraries

### **pandas**: Library for data manipulation and analysis.
Data Loading

### **pd.read_csv("apple_sales_2024.csv"):** Load the dataset into a DataFrame.
Exploratory Data Analysis (EDA)

### **df.shape:** Check dataset dimensions (rows and columns).
### **df.head(n), df.tail(n):** Display the first or last n rows.
### **df.info():**  Get an overview of the dataset, including column types and null values.
### **df.describe():** Generate descriptive statistics for numerical columns.
# **Renaming Columns**

df.rename(columns={"old_name": "new_name"}, inplace=True): Rename specific columns.
Column and Data Selection

**Access a single column:** df['ColumnName'].
**Access multiple columns:** df[['Column1', 'Column2']].
# **Data Aggregation**

**value_counts():** Count occurrences of unique values.
# **Calculate statistics:**
**Mean:** df['ColumnName'].mean()
**Median:** df['ColumnName'].median()
**Mode:** df['ColumnName'].mode()
# **Handling Missing Data**

**df.isnull():** Identify missing values.
**df.isnull().sum():** Count missing values per column.
**Filter rows with missing values:** df[df['ColumnName'].isnull()].
# **Data Grouping**

**df.groupby('ColumnName').describe():** Group data by a column and generate descriptive statistics.
# **Visualization**

# **Plot data distributions:**
**Pie chart:** df['ColumnName'].value_counts().plot(kind="pie")
**Bar chart:** df['ColumnName'].value_counts().plot(kind="bar")
**Density plot:** df['ColumnName'].value_counts().plot(kind="density")
Feel free to extend the notebook for advanced preprocessing tasks or additional visualizations as needed.