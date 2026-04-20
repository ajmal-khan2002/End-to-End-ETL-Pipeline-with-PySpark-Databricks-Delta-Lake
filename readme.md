# End-to-End ETL Pipeline with PySpark

A modular, production-ready Data Engineering pipeline built on **Databricks** and **PySpark**. This framework utilizes the **Strategy Design Pattern**, allowing for decoupled, testable, and highly maintainable transformation logic across 46M+ records.

### 🛠 Tech Stack
![PySpark](https://img.shields.io/badge/PySpark-FF69B4?style=for-the-badge&logo=apache-spark&logoColor=white)
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=for-the-badge&logo=databricks&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

---

# 🏗️ ETL Architecture
<img width="465" height="181" alt="Screenshot 2026-03-06 151712" src="https://github.com/user-attachments/assets/dd7277ce-8417-495e-80b4-d7e0d3965f5d" />

*The pipeline follows the industry-standard **Medallion Architecture**, ensuring data quality and traceability from raw ingestion to analytical reporting.*

---

## 🚀 Engineering Features
* **Strategy Pattern:** Decoupled business logic for high maintainability.
* **Schema Enforcement:** Strict `StructType` contracts to prevent downstream failures.
* **Production-Grade Logging:** Custom `logging_config` for observability and troubleshooting.
* **Modular ETL:** Clean separation of concerns (Extraction, Transformation, Loading).

## 🧩 Engineering Challenges
* **Scalable Joins:** Implemented `broadcast()` joins to eliminate network shuffles.
* **Code Modularity:** Used Strategy Pattern to avoid "spaghetti code."
* **Data Integrity:** Proactive filtering of 'Unknown' categories and null values at the ingestion layer.

---

## 📂 Project Structure
/<br>
├── workflow/<br>
│ ├── logging_config.ipynb # Centralized logging logic<br>
│ └── extractor.ipynb # Data ingestion framework<br>
├── transform.ipynb # Strategy-based transformation classes<br>
├── loader.ipynb # Sink and load operations<br>
└── analysis.ipynb # Orchestration/Execution entry point<br>


---

## 🚀 How to Run

1. **Configure Environment:** Ensure the Databricks environment has access to the defined file paths.  

2. **Initialize Logging:** Run the logging_config notebook.  

3. **Execute Workflow:** Use the WorkFlowRunner in analysis.ipynb to instantiate and run desired transformation classes.  
