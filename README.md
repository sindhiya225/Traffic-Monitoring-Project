[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

# Traffic Monitoring and Accident Prediction Project

## Overview
A PySpark-based system to monitor traffic, detect congestion, and predict accident risks using the UK Traffic Accidents dataset and simulated streaming data. Achieved AUC 0.92 with a Random Forest model.

## Setup
1. Open `Traffic_Monitoring_Project.ipynb` in Google Colab.
2. Install dependencies: `!pip install pyspark==3.4.0 pandas matplotlib seaborn`
3. Upload the UK Traffic Accidents dataset CSV.
4. Run all cells.

## Deliverables
- **Notebook**: `Traffic_Monitoring_Project.ipynb`
- **Architecture Diagram**: `architecture_diagram.md` (render with Mermaid)
- **ETL & Streaming Pipelines**: Included in notebook
- **ML Model**: Random Forest with AUC 0.92
- **Dashboard**: Visualizations (traffic_density.png, roc_curve.png, confusion_matrix.png)
- **Report**: `final_report.md`

## Results
- AUC: 0.92
- Visualizations: [Insert screenshots of plots]

## Challenges Overcome
- Resolved `IllegalArgumentException`, `PySparkTypeError`, and `AttributeError` in PySpark ML pipeline.
- Balanced imbalanced dataset (87% non-severe, 13% severe) using oversampling.
