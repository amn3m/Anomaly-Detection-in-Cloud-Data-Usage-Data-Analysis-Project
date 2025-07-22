# Anomaly Detection in Cloud Service Data Usage

This repository contains the code and analysis for the **Anomaly Detection in Data Usage** project. The study presents a comprehensive analysis of data usage patterns for three major cloud service providers—Amazon Web Services (AWS), Google Web Services (GWS), and Apple Web Services—to identify anomalies indicating potential security breaches or technical issues.

## Project Overview

The exponential growth of cloud computing necessitates robust monitoring of data usage to ensure operational efficiency and security. This project leverages machine learning techniques to analyze historical data from two French cities, Dijon and Toulouse, to detect anomalous patterns. By identifying significant deviations from normal behavior, we provide actionable insights for enhancing cloud security and performance.

## Key Features

*   **Multi-Provider Analysis:** Simultaneously analyzes and compares data usage patterns across AWS, GWS, and Apple Web Services.
*   **Advanced Anomaly Detection:** Employs a suite of machine learning models, including Random Forest, KNN, and Clustering, to detect outliers and unusual patterns.
*   **Time-Series Forecasting:** Utilizes a KNN-based model to forecast future traffic and identify behavioral anomalies in real-time.
*   **Security Threat Identification:** Pinpoints specific high-risk time windows where security breaches are most likely to occur based on data usage volatility.
*   **Comprehensive Visualization:** Features detailed plots, heatmaps, and cluster visualizations to interpret model predictions and data trends effectively.

##  Methodology & Technologies

The project follows a structured methodology to ensure accurate and insightful analysis:

1.  **Data Aggregation:** Raw data was aggregated into 30-minute intervals to balance granularity and reduce data volume for time-series analysis.
2.  **Outlier Detection:** The Interquartile Range (IQR) method was used to identify statistical outliers, which were retained as potential indicators of significant anomalies.
3.  **Machine Learning Models:**
    *   **Random Forest Regression:** Used to predict usage, analyze prediction errors, and understand feature importance, helping to uncover hidden patterns and potential threats.
    *   **K-Nearest Neighbors (KNN) Regression:** Implemented a distance-based model to flag the top 5% of anomalies, effectively identifying data points that deviate significantly from their neighbors.
    *   **Unsupervised Clustering:** Grouped similar data usage patterns to highlight outliers and clusters with high variability, which are often associated with security risks.

*   **Technologies:** `Python`
*   **Libraries:** `Pandas`, `Scikit-learn`, `Matplotlib`, `Seaborn`

## Dataset

The analysis was performed on the **NetMob 2023 Challenge dataset**, which provides high-resolution, service-level mobile data traffic from the cities of Paris and Marseille. This project focused on the data corresponding to Dijon and Toulouse.

## Key Findings

*   The machine learning models successfully identified anomalous usage spikes and drops correlated with external events and potential security vulnerabilities.
*   Clustering analysis effectively isolated high-risk periods, such as **11:00 for AWS in Toulouse** and **14:30 for GWS in Toulouse**, where security breaches were most likely.
*   The KNN regression model proved highly effective in pinpointing significant anomalies by identifying the top 5% of deviating data points.
*   The study confirmed that regional events and user behaviors cause significant variations in cloud usage patterns, underscoring the need for location-specific monitoring.

## Authors

*   Ahmed Abdelmoneim
*   Maryam Mohamed
*   Seif Kassab
*   NourEldeen Ayman
*   Farida Salah
