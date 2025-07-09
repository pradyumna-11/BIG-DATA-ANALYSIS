# BIG-DATA-ANALYSIS

"COMPANY" : CODTECH IT SOLUTIONS

"NAME" : SIKHAKOLLI PRADYUMNA

"INTERN ID" : CT08DN583

"DOMAIN" : DATA ANALYSIS

"DURATION" : 8 WEEKS

"MENTOR" : NEELA SANTOSH

## 📌 Task 1: Big Data Analysis Using PySpark to Demonstrate Scalability

### 📝 Overview

The primary objective of this task is to **analyze a large dataset using distributed data processing tools like PySpark or Dask**. Big data analysis involves processing and extracting insights from datasets that are too large to be handled efficiently using traditional data analysis tools like pandas. In this project, we utilize **PySpark** (Apache Spark’s Python API) to demonstrate scalability, speed, and efficient memory management while performing real-time data transformations and aggregations on large datasets.

This task simulates a real-world data engineering or data science scenario where analyzing large-scale structured data requires distributed computing. By leveraging PySpark, we can handle millions of records, perform grouping, filtering, aggregations, and gain meaningful business insights that wouldn't be possible with in-memory libraries alone.

---

### ⚙️ Tools & Technology Used

* **Python 3**
* **PySpark**: Python API for Apache Spark
* **Google Colab / Jupyter Notebook** for script execution
* **Pandas** (for visualization of small samples, where required)
* **Matplotlib / Seaborn** (optional, for data visualization)

---

### 📂 Dataset

We used a publicly available CSV dataset (like the NYC Taxi Trip data, Amazon Reviews, or a simulated large dataset like Titanic replicated multiple times for scaling). The dataset was large enough to showcase how PySpark handles memory and compute using lazy evaluation and distributed execution.

The dataset typically included:

* Categorical columns: gender, class, survival, etc.
* Numerical columns: fare, age, distance, etc.
* Nullable columns for data cleaning scenarios

---

### 🔍 Objectives

* Load and process large-scale data using Spark
* Perform schema inference and exploration using `SparkSession`
* Apply big data transformations: filtering, grouping, joins
* Aggregate metrics (e.g., survival rate, average fare per class, age group distribution)
* Identify performance benefits of distributed processing
* Optionally visualize small sample summaries using Pandas or Matplotlib

---

### 🔧 Approach

1. **Setup Spark Session**
   Using `SparkSession.builder`, we initialized the Spark engine in local mode to run distributed processing on a single machine.

2. **Data Loading**
   A large dataset in CSV format was read using `spark.read.csv(...)` with header inference and automatic schema detection enabled.

3. **Data Cleaning**
   We handled null values, filtered unusable records, and casted columns to appropriate data types.

4. **Transformations & Aggregations**

   * Grouped data by categories like class, gender, and survival
   * Calculated mean, count, and other statistics using `.groupBy()` and `.agg()`
   * Used PySpark’s `withColumn`, `filter`, and `select` for efficient processing

5. **Insights Extraction**
   Derived actionable insights like:

   * Average fare by passenger class
   * Survival rate by gender
   * Age distribution among classes
   * Passenger count trends

6. **Visualization (Optional)**
   For small sample subsets, we converted Spark DataFrames to pandas using `.toPandas()` and visualized with `matplotlib` or `seaborn`.

---

### 📈 Insights & Results

After processing, the analysis revealed:

* Clear differences in survival rates across gender and class
* Average fare varied significantly between passenger classes
* Missing data in age and cabin columns needed to be handled for reliable modeling
* PySpark efficiently handled a dataset with hundreds of thousands of rows with no performance issues, demonstrating its scalability

---

### 🚀 Scalability Demonstrated

Unlike pandas, which loads the entire dataset into memory, PySpark:

* **Processes data lazily** (operations are not executed until an action like `show()` or `collect()` is called)
* **Distributes data and computation** across multiple cores or machines
* **Manages memory** more efficiently for large datasets

This task demonstrated how PySpark can scale to real-world data sizes, making it ideal for production-level data processing pipelines in big data environments.

---

### 📤 Deliverables

* A single `.ipynb` notebook (or `.py` script) with:

  * All data processing steps
  * Code comments and section headers
  * Insights printed at the end of the notebook
  * Optional visualizations of aggregated data
* Dataset used (or reference to public dataset link)

## Output:

<img width="748" height="150" alt="Image" src="https://github.com/user-attachments/assets/2eb07cca-4d2e-4da6-87a0-1d0f0830cd93" />


<img width="1314" height="323" alt="Image" src="https://github.com/user-attachments/assets/79e3fb68-8a17-412d-a4d2-0e4215c23c06" />


<img width="215" height="104" alt="Image" src="https://github.com/user-attachments/assets/c1ea82f3-a882-47ac-8265-fcdeedbff1de" />


<img width="216" height="96" alt="Image" src="https://github.com/user-attachments/assets/4f320eb3-0932-490f-a364-82784080769d" />


<img width="531" height="393" alt="Image" src="https://github.com/user-attachments/assets/288ccb45-789b-4b21-80f7-2353bcba5e86" />


<img width="531" height="427" alt="Image" src="https://github.com/user-attachments/assets/1fa6b75b-6889-436a-af3a-7e082950a137" />


<img width="442" height="427" alt="Image" src="https://github.com/user-attachments/assets/c7712c60-c419-4c18-bdf5-d8726f7e5061" />


<img width="695" height="470" alt="Image" src="https://github.com/user-attachments/assets/97a87c92-0ebb-4da7-984c-7e6497d39c36" />


<img width="706" height="597" alt="Image" src="https://github.com/user-attachments/assets/b02dd5d5-f437-4f09-abec-a92572c9d63f" />


<img width="698" height="470" alt="Image" src="https://github.com/user-attachments/assets/e859fbbc-1a2b-4e11-ab3a-4b7675c86f50" />


<img width="686" height="470" alt="Image" src="https://github.com/user-attachments/assets/9c76a395-fea4-4936-adc5-a326941b78d1" />
