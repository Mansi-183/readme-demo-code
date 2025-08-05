# readme-demo-code
This repository contains sample code for Business and Data Analysis tasks using Python and SQL. It includes basic data exploration, reporting, and visualization with mock data. The goal is to showcase practical analysis techniques and share self-contained examples for portfolio or learning use.
## 📊 Data Analyst Sample Code

This code demonstrates a simple data analysis using Python and pandas with in-line sample data.

```python
import pandas as pd
import matplotlib.pyplot as plt

# Sample data created within code
data = {
    'Region': ['East', 'West', 'North', 'South'],
    'Sales': [100, 150, 200, 120]
}

df = pd.DataFrame(data)

# Plotting sales by region
df.groupby('Region')['Sales'].sum().plot(kind='bar')
plt.title('Sales by Region')
plt.xlabel('Region')
plt.ylabel('Total Sales')
plt.show()
