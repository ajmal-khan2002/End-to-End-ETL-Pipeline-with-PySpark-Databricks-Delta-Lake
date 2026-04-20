## End-to-End ETL Pipeline with PySpark

A modular, production-ready Data Engineering pipeline built on Databricks and PySpark. This framework is designed with a Strategy Design Pattern, allowing for decoupled, testable, and highly maintainable transformation logic across 46M+ records.

---

# ETL Architecture

<img width="465" height="181" alt="Screenshot 2026-03-06 151712" src="https://github.com/user-attachments/assets/dd7277ce-8417-495e-80b4-d7e0d3965f5d" />

---

## 🏗️ Core Architecture

The pipeline is structured into three distinct layers to ensure separation of concerns:

- **Extraction Layer:** Modular Extractor classes to ingest raw data with strict schema enforcement.  
- **Transformation Layer:** A robust library of Transformer classes following the Strategy Pattern, enabling independent logic development.  
- **Loading & Orchestration:** A centralized WorkflowRunner that manages the execution flow, logging, and data sink operations.  

---

## ⚙️ Engineering Features

- **Strategy Pattern Implementation:** Transformations are encapsulated as individual classes. Adding new business logic requires only creating a new class, preventing "Spaghetti Code."  

- **Schema Enforcement:** Rigid data contracts using PySpark StructType ensure data quality at the point of ingestion, preventing downstream type-mismatch failures.  

- **Production-Grade Logging:** Custom logging_config integration provides detailed execution logs (INFO, ERROR) to local directories for efficient production troubleshooting.  

- **Modular ETL:** Clean separation of Extraction, Transformation, and Loading, making the codebase highly unit-testable.  

---

## 📂 Project Structure
/
├── workflow/
│ ├── logging_config.ipynb # Centralized logging logic
│ └── extractor.ipynb # Data ingestion framework
├── transform.ipynb # Strategy-based transformation classes
├── loader.ipynb # Sink and load operations
└── analysis.ipynb # Orchestration/Execution entry point


---

## 🚀 How to Run

1. **Configure Environment:** Ensure the Databricks environment has access to the defined file paths.  

2. **Initialize Logging:** Run the logging_config notebook.  

3. **Execute Workflow:** Use the WorkFlowRunner in analysis.ipynb to instantiate and run desired transformation classes.  
