# TransJakarta Ridership Data Analysis

## Project Title

**TransJakarta Ridership and Revenue Optimization Analysis**

## Project Overview

This project provides a comprehensive analysis of TransJakarta's ridership data for April 2023. TransJakarta is Jakarta’s primary Bus Rapid Transit (BRT) system, serving millions of commuters across various corridors with a flat fare structure. By analyzing this dataset, we aim to extract actionable insights that can inform operational strategies, improve passenger experience, and increase revenue.

The key objectives include:

* Identifying peak usage hours and load patterns
* Analyzing route-specific performance and terminal activity
* Uncovering demographic trends and underutilized services
* Providing strategic recommendations for route optimization and service adjustments

The analysis includes data visualization, geospatial mapping, and AI-powered natural language querying to enhance understanding and decision-making.

---

## Dataset

* **Source**: Public dummy dataset representing TransJakarta trip data
* **Link**: [Public Kaggle Transjakarta](https://www.kaggle.com/datasets/dikisahkan/transjakarta-transportation-transaction/data) or [dfTransjakarta.csv on GitHub](https://github.com/dikisahkan/jupyternotebook/blob/main/dummyDatasetTransjakarta/dfTransjakarta.csv)
* **Size**: Approximately 37,000 records
* **Contents**: Includes fields such as date, terminal origin/destination, passenger count, revenue, and rider demographics

---

## Insights & Findings

The analysis reveals several important insights:

* **Peak Usage Times**: Highest passenger volumes occur during weekday mornings (06:00–08:00) and evenings (16:00–18:00), indicating strong commuter patterns.
* **Revenue Trends**: Terminals such as Harmoni, Blok M, and Dukuh Atas consistently generate the highest revenues, linked to central business areas.
* **Overcrowding Indicators**: Load imbalances exist on certain corridors and during peak hours, pointing to a need for vehicle reallocation or schedule adjustment.
* **Demographic Patterns**: Riders aged 20–34 dominate the user base, with relatively low ridership among seniors (60+).
* **Route Optimization Opportunities**: Underused feeder routes and corridors can benefit from promotion or rerouting strategies.
* **Spatial Visualization**: Mapping supports identification of service coverage gaps and demand clusters.

---

## AI Support

To enhance the analysis, the project uses AI tools to provide real-time assistance and exploratory capabilities:

* **LangChain Agents**: Enable natural language question answering directly in the notebook. For example, users can ask:
  *“Which terminal has the lowest revenue on weekends?”*
* **Replicate API Integration**: Used to interpret user queries, generate summaries, and suggest visualizations automatically.
* **AI Use Cases**:

  * Auto-generation of insights
  * Data storytelling support
  * Fast identification of key trends via conversational interface

This integration enables users to interact with the dataset more intuitively and extract insights with minimal manual exploration.

---