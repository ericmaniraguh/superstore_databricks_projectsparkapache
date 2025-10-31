
# **Project Title:** Sales Analytics Dashboard with PySpark

## **Project Overview**
#### *analyzing sales data, calculating key metrics, and generating dashboards using PySpark and SQL*
This project analyzes sales data from the `cleaned_superstore_final_view` dataset to extract actionable business insights. Using **PySpark** and **SQL**, it calculates key metrics such as top customers, most profitable regions, sales trends, and customer behavior. The analysis helps in identifying high-value customers, profitable regions, and potential opportunities for revenue growth.

---

## **Key Features / Metrics**

The project computes and visualizes the following metrics:

1. **Total Customers, Sales, and Profit**

   * Aggregate number of customers, total sales, and total profit over a given date range.

2. **Most Profitable Region and Country**

   * Identifies the top regions and countries contributing to revenue and profit.

3. **Top Customers by Total Sales per City**

   * Ranks customers within each city based on total sales and identifies the highest-value customers.

4. **Additional Metrics** (examples based on your project)

   * Monthly sales trends
   * Profitability per product category
   * Customer order frequency

---

## **Technologies Used**

* **PySpark**: Data processing and aggregation.
* **Spark SQL**: Writing SQL queries on Spark DataFrames.
* **Python**: Orchestration, data manipulation, and display.
* **Jupyter / Databricks**: Interactive development and visualization.

---

## **Installation & Setup**

1. **Clone the repository**:

   ```bash
   git clone <your-repo-url>
   cd <project-folder>
   ```

2. **Set up PySpark environment** (if not using Databricks):

   ```bash
   pip install pyspark
   ```

3. **Load your dataset** into a Spark DataFrame:

   ```python
   df_final_cleaned = spark.read.format("csv") \
       .option("header", "true") \
       .option("inferSchema", "true") \
       .load("cleaned_superstore_final_view.csv")
   ```

---

## **Usage**

* Run the metrics scripts in order:

  1. Metric 1: Total Customers, Sales, and Profit
  2. Metric 6: Most Profitable Region and Country
  3. Metric 10: Top Customer by Total Sales per City

* Metrics can be displayed using:

  ```python
  display(metric_dataframe)
  ```

* SQL queries can be executed directly on Spark DataFrames using:

  ```python
  df_final_cleaned.createOrReplaceTempView("df_final_cleaned")
  spark.sql("SELECT ... FROM df_final_cleaned WHERE ...")
  ```

---

## **Folder Structure**

```
project-root/
│
├── data/                     # Dataset CSV files
├── notebooks/                # Jupyter/Databricks notebooks
├── scripts/                  # PySpark Python scripts for metrics
├── README.md                 # Project documentation
└── requirements.txt          # Python dependencies
```

---

## **Contributing**

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m "Add feature"`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

Here is a shorter, clean version using **inline Markdown link formatting**:

---

### **Databricks Git Integration Link**

[Click here to open Databricks with Git integration enabled](https://dbc-a3d6af82-c511.cloud.databricks.com/browse/folders/home?addGit=&o=4075981409173999&gitUrl=https%3A%2F%2Fgithub.com%2Fericmaniraguh%2Fsuperstore_databricks_projectsparkapache.git&gitProvider=gitHub)

This link opens Databricks with Git integration enabled and allows contributors to clone the repository directly into their workspace.

---

## **License**

This project is licensed under the MIT License.

---

If you want, I can also **write a shorter, more marketing-friendly README** with badges, images, and examples of dashboards that makes it look **professional on GitHub**.

Do you want me to do that?
