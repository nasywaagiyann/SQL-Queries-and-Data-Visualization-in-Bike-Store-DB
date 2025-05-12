# SQL Queries and Data Visualization in Bike Store DB

## 📌 Description

This project showcases SQL queries and data visualizations based on the Bike Store Database. The dataset is loaded from CSV files into a SQLite database and analyzed using Python libraries such as Pandas and Matplotlib. It aims to explore insights about sales, stock, and staff performance across multiple bike store locations.

## 📁 Datasets Used

The following tables are included:

* `products`
* `brands`
* `categories`
* `order_items`
* `orders`
* `staffs`
* `stores`
* `customers`
* `stocks`

## 🔧 Technologies

* Python (Pandas, NumPy, Matplotlib)
* SQLite (via `sqlite3`)
* Google Colab (Jupyter Notebook)
* SQL (for querying data)

## 📊 Analysis & Visualizations

1. **Stock Quantity by Category and Store**

   * Merged data from `products`, `categories`, `stocks`, and `stores`.
   * Visualization: Bar chart.

2. **Number of Order Items by Category from Each Store**

   * Joined `categories`, `products`, `order_items`, `orders`, and `stores`.
   * Visualization: Bar chart.

3. **Number of Order Items by Category from Baldwin Bikes Only**

   * Filtered for `"Baldwin Bikes"` store.
   * Visualization: Bar chart.

4. **Total Sales per Month per Store**

   * Performed for three stores:

     * `Santa Cruz Bikes`
     * `Rowlett Bikes`
     * `Baldwin Bikes`
   * Calculated using `quantity * list_price * (1 - discount)`.
   * Visualization: Line chart.

5. **Staff with the Highest Number of Orders**

   * SQL query using JOIN and aggregation to count orders per staff member.

## 📷 Sample Visualizations

* Bar chart for stock by category and store
* Line chart for total monthly sales
* SQL-based ranking of top-performing staff

## 🏁 How to Run

1. Make sure all CSV files (`products.csv`, `orders.csv`, etc.) are available in the directory.

2. Open and run the notebook in Google Colab or Jupyter.

3. Install required libraries if needed:

   ```python
   import pandas as pd
   import numpy as np
   import matplotlib.pyplot as plt
   import sqlite3
   ```

4. Run each code cell sequentially to reproduce the analysis.
