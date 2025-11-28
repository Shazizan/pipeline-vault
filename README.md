# 📦 pipeline-vault: Centralised ETL Experiment Data Repository

**pipeline-vault** is a storage repository for all processed datasets generated from my ETL (Extract–Transform–Load) experiments.  
All data stored here is **loaded via the GitHub API** and serves as the **processed data repository (target system)** for my projects.

This repo is used together with **Google Colab (Jupyter Notebook)**, where I perform data extraction and transformation using **Python**, mainly through:

- **Pandas** for small/medium datasets  
- **PySpark** for large-scale or distributed data processing

---

## 🔄 ETL Workflow Overview

### 1. Extraction
- During this experimentation, data is gathered from multiple sources to serve as the foundation for ETL processes.  
- Using Google Colab (Jupyter Notebook) with **Pandas** and **PySpark**, all raw datasets are uploaded into the source repository, organised under the folder named [`data`](https://github.com/Shazizan/data), which acts as the central data storage for this project.

**2. Transformation**  
- Standard cleaning (handling nulls, type casting, filtering).  
- Enrichment and structuring using both Pandas and PySpark functions.
- All the processes and code scripts can be viewed in my [portfolio](https://github.com/Shazizan/portfolio) repository.

**3. Loading (via GitHub API)**  
- The final transformed datasets are uploaded into this repository.  
- Stored in multiple formats: **CSV**, **Parquet** and **JSON**.

This repo acts as a **vault** for all processed outputs used across different ETL pipeline tests.

---

## 📁 Data Formats Stored in This Repository

| Format   | Description | Characteristics | Best Use Cases | Tools / Libraries |
|---------|-------------|----------------|----------------|-----------------|
| **CSV** | Comma-Separated Values, a simple text-based tabular format | - Easy to read and human-friendly<br>- Lightweight and universal | - Small datasets<br>- Quick inspection<br>- Data exchange between tools | Pandas, Excel, Python CSV module |
| **Parquet** | Columnar, compressed binary format optimized for big data | - Highly compressed → smaller storage<br>- Columnar → faster queries<br>- Optimized for distributed processing | - Large-scale datasets<br>- Analytics workloads<br>- PySpark optimization | PySpark, Hadoop, Databricks |
| **JSON** | JavaScript Object Notation, flexible hierarchical format | - Supports nested structures (objects, arrays)<br>- Semi-structured and human-readable<br>- More verbose than CSV | - API responses<br>- Document-style or semi-structured data<br>- Logs or configuration files | Pandas, Python `json` module, APIs |


---

## 📊 Quick Comparison (CSV vs Parquet vs JSON)

| Feature            | CSV                     | Parquet                         | JSON                          |
|-------------------|-------------------------|---------------------------------|-------------------------------|
| Structure         | Tabular (rows/columns)  | Columnar compressed             | Semi-structured (nested)      |
| Readability       | ⭐ Very easy             | ❌ Not human-readable           | ⭐ Easy, but verbose           |
| File Size         | Large                   | Small (high compression)        | Medium                        |
| Best For          | Simple datasets         | Big data + analytics            | API / nested data             |
| Tools             | Pandas, Excel           | PySpark, Hadoop, Databricks     | APIs, NoSQL, Logs             |

---

## ⚙️ Technology Used

- **Google Colab (Jupyter Notebook)**  
- **Python**  
  - **Pandas** for local data manipulation  
  - **PySpark** for distributed processing  
- **GitHub API** for automated upload of processed data  
- **GitHub** as the storage vault

---

## 🎯 Purpose of This Repository

- Centralised storage for **all ETL experimental outputs**  
- Allows versioning and tracking of data changes  
- Supports multi-format dataset exploration  
- Helps me learn and practice real-world data engineering workflows  

---

If you have suggestions or want to collaborate, feel free to open an issue or pull request! 🚀
