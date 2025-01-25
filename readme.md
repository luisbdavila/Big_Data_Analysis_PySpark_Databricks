# Big Data Analysis Using PySpark on Databricks

## Project Overview
This project demonstrates the use of PySpark and Databricks for Big Data analysis by addressing key challenges across three domains: real estate price prediction, NYC taxi trip graph analysis, and stock market streaming. The project showcases the 4 V's of Big Data—Volume, Variety, Velocity, and Veracity—while leveraging Spark’s advanced functionality like RDDs, DataFrames, SparkSQL, machine learning pipelines, graph analytics, and streaming.

## Objectives
1. Apply PySpark to process and analyze datasets across different domains.
2. Showcase advanced Spark functionality, including machine learning, graph analysis, and real-time streaming.
3. Extract meaningful insights and demonstrate how Big Data tools can solve real-world challenges.
4. Optimize workflows to handle data at scale, demonstrating scalability and performance.

## Problem Statement
Big Data poses significant challenges in processing, analyzing, and deriving insights from vast, diverse datasets in real-time. This project aimed to address these challenges by using PySpark to:
1. Build a machine learning model for real estate price prediction.
2. Analyze NYC taxi trips to uncover traffic patterns and hotspots using graph analytics.
3. Simulate real-time stock market analysis with Spark Streaming.

## Methodology
### Tools
- **PySpark**: For distributed processing and advanced analytics.
- **Databricks**: As the development environment for managing data pipelines, ML, and graph frameworks.
- **SparkSQL, MLlib, GraphFrames, and Streaming APIs**: For domain-specific implementations.

### Use Cases
1. **Real Estate Price Prediction (ML)**:
   - Dataset: Portuguese real estate listings (114,623 rows).
   - Key Steps:
     - Data cleaning, outlier removal, and imputation using Random Forest.
     - Feature scaling and one-hot encoding with pipelines.
     - Model comparison: Gradient Boosted Trees, Random Forest, Linear Regression, Neural Networks.
   - Outcome:
     - Best model: Random Forest (RMSE: €259,689).

2. **NYC Taxi Graph Analysis (Graph)**:
   - Dataset: NYC taxi trip data (3,158,863 rows for December 2023).
   - Key Steps:
     - Integrated taxi zones and trip datasets using SparkSQL.
     - Applied PageRank, Label Propagation, and degree analysis with GraphFrames.
     - Visualized borough connectivity with NetworkX.
   - Insights:
     - Manhattan has the highest connections, with hotspots in high-cost living areas and tourist destinations.
     - Seasonal events (e.g., Christmas and New Year’s Eve) impact taxi demand.

3. **Stock Market Streaming (Streaming)**:
   - Dataset: Simulated stock data (e.g., Microsoft stock prices).
   - Key Steps:
     - Data ingestion using Spark Streaming and Yahoo Finance API.
     - Calculated Bollinger Bands, volatility, and outliers in 1-hour time windows.
     - Watermarking to handle late-arriving data.
   - Outcome:
     - Provided a scalable and dynamic pipeline for real-time financial analysis.

### Challenges and Solutions
- **Cluster Crashes**:
  - Solution: Reduced memory usage by saving intermediate variables to disk.
- **Handling Small Datasets**:
  - Solution: Ensured all methods and workflows are scalable for large datasets.

## Key Insights
1. **Machine Learning**:
   - Real estate prices are influenced by location (Lisbon), property type, and features like elevators.
2. **Graph Analysis**:
   - High-income individuals frequently travel between upscale zones, with distinct patterns for Christmas and New Year’s.
3. **Streaming**:
   - Real-time analysis highlights market volatility and helps identify significant price movements.

## Deliverables
1. **Notebooks**:
   - Three notebooks showcasing ML, graph analysis, and streaming implementations.
2. **Report**:
   - Summarizes methodology, insights, and conclusions for a management audience.

## Conclusion
This project demonstrates the power of PySpark and Databricks in addressing diverse Big Data challenges. By combining machine learning, graph analytics, and streaming, it delivers actionable insights across industries, showcasing scalability, flexibility, and efficiency.
