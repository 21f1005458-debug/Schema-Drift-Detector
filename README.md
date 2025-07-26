# Schema-Drift-Detector
Schema Drift Detector for Data Pipelines

### 📄 README.md
```markdown
# 🧬 Schema Drift Detector with PySpark

## 🧠 Overview
This project detects schema drift in incoming datasets by comparing them with a predefined baseline schema. It identifies added/removed columns and datatype changes to prevent pipeline breakages.

## 📊 Features
- Compare real-time schema vs baseline
- Identify column/type mismatches
- JSON report output for audit and alerting
- SQLite logging for schema change history

## 🛠️ Tech Stack
- PySpark
- Python (json, logging)
- SQLite (optional)

## 📁 Folder Structure
- `data/`: Incoming dataset to check
- `baseline_schema/`: Expected schema definition
- `scripts/`: Drift detection logic
- `output/`: Drift reports

## ▶️ Run the Detector
```bash
spark-submit scripts/drift_detector.py --baseline baseline_schema/baseline_schema.json --input data/incoming_data.csv
