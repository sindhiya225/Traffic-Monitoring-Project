# Traffic Monitoring and Accident Prediction Project

## Overview
This project implements a real-time traffic monitoring and accident prediction system using PySpark on Google Colab. It processes historical and simulated streaming traffic data to detect congestion, predict accident risks, and visualize traffic patterns.

## Architecture
- **Data Sources**: UK Traffic Accidents Dataset (CSV), simulated streaming data (JSON-like).
- **Ingestion**: Spark DataFrames for batch, Python generator for streaming simulation.
- **Processing**: ETL pipeline with Spark SQL, streaming processing for congestion detection.
- **ML Model**: Random Forest for accident probability prediction.
- **Visualization**: Matplotlib/Seaborn for traffic density, ROC curve, and confusion matrix.

## Challenges Overcome
- Resolved `IllegalArgumentException` by correcting string-to-numeric mapping of `Accident_Severity`.
- Fixed `PySparkTypeError` in oversampling by using a float fraction, balancing the dataset (87% non-severe, 13% severe).
- Corrected `AttributeError` in model saving by using the appropriate ML model API.

## Deliverables
- PySpark notebooks for ETL, streaming, ML, and visualization.
- Visualizations of traffic density, ROC curve, and confusion matrix.
- Random Forest model with AUC 0.92.
- Comprehensive report.

## Tools
- **Language**: Python, PySpark
- **Platform**: Google Colab
- **Libraries**: Pandas, Matplotlib, Seaborn, Spark MLlib

## Results
- Achieved AUC 0.92 in accident prediction.
- Successfully detected low-speed clusters as congestion indicators.
- Visualized traffic patterns, model performance (ROC curve), and prediction accuracy (confusion matrix).

## Conclusion
This project demonstrates proficiency in big data processing, machine learning, and visualization using PySpark. It is scalable for real-world traffic monitoring applications.

## Future Work
- Integrate real Kafka streaming.
- Deploy on Databricks for production.
- Enhance visualizations with interactive dashboards.