# TransJakarta Ridership and Revenue Optimization Analysis

In today's data-driven world, even a single row of data may seem meaningless at first glance. But when collected over time, like a month, can reveal deeper insights.

This project explores TransJakarta's ridership data, including tap-in and tap-out history sourced from public dataset of [Kaggle](https://www.kaggle.com/datasets/dikisahkan/transjakarta-transportation-transaction/data). As transactions accumulate daily, this data becomes a critical asset for operational insights and service evaluation.

To simplify and enhance the analysis, IBM’s AI-powered tools were utilized for tasks such as data summarization and classification, enabling us to conduct this analysis with minimal coding knowledge through clear and structured instructions.

## Table of Contents

* [Project Overview](#project-overview)
* [Dataset](#dataset)
* [How to Use This Project](#how-to-use-this-project)

  * [Prerequisites](#prerequisites)
  * [Setup Instructions](#setup-instructions)
* [Analytical Workflow](#analytical-workflow)

  * [1. Business Understanding](#1-business-understanding)
  * [2. Data Understanding](#2-data-understanding)
  * [3. Data Preprocessing](#3-data-preprocessing)
  * [4. Exploratory Data Analysis (EDA)](#4-exploratory-data-analysis-eda)
  * [5. Insight Extraction](#5-insight-extraction)
* [AI Support: IBM Granite-3.3-8B-Instruct](#ai-support-ibm-granite-338b-instruct)

  * [Limitations](#limitations)
* [Insights & Findings](#insights--findings)
* [Documentation](#documentations)


## Project Overview

This project provides a comprehensive analysis of TransJakarta's ridership data for April 2023. TransJakarta is Jakarta’s primary Bus Rapid Transit (BRT) system, serving millions of commuters across various corridors with a flat fare structure. By analyzing this dataset, we aim to extract actionable insights that can inform operational strategies, improve passenger experience, and increase revenue.

The key objectives include:

* Identifying peak usage hours and load patterns
* Identify high-performing corridors and peak ridership patterns.
* Uncovering demographic trends
* Providing strategic recommendations for operational

The analysis includes data visualization, geospatial mapping, and AI-powered natural language querying to enhance understanding and decision-making.


## Dataset

* **Source**: Public dummy dataset representing TransJakarta trip data
* **Link**: [Public Kaggle Transjakarta](https://www.kaggle.com/datasets/dikisahkan/transjakarta-transportation-transaction/data) or [dfTransjakarta.csv on GitHub](https://github.com/dikisahkan/jupyternotebook/blob/main/dummyDatasetTransjakarta/dfTransjakarta.csv)
* **Size**: Approximately 37,000 records
* **Contents**: Includes fields such as date, terminal origin/destination, passenger count, revenue, and rider demographics


## How to Use This Project

### Prerequisites

* Python 3.8+
* Jupyter Notebook
* Python libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `folium`, `geopandas`, `ibm_granite`, `replicate`

### Setup Instructions

1. **Clone the repository:**

   ```bash
   git clone https://github.com/hudiyaresa/LLM-Guided-TransJakarta-Insights/
   cd LLM-Guided-TransJakarta-Insights
   ```

2. **Run the analysis notebook:**

   ```bash
   jupyter notebook Transjakarta_ridership_data_analysis.ipynb
   ```

Or you can use [Google Colab](https://colab.research.google.com/) to upload and run this [Jupyter Notebook](https://github.com/hudiyaresa/LLM-Guided-TransJakarta-Insights/blob/main/Transjakarta_ridership_data_analysis.ipynb) files


## Analytical Workflow

### 1. **Business Understanding**
- Define primary goals:
  - Improve bus scheduling and comfort.
  - Identify corridor-level revenue and ridership hotspots.
  - Explore marketing potential based on user demographics.

### 2. **Data Understanding**
- Load and explore key attributes:
  - Corridor ID, stop names, timestamps, payment info.
  - Basic statistics on fare, trip duration, and passenger profiles.

### 3. **Data Preprocessing**
- Convert string-based dates to proper `datetime` format for tap-in and tap-out.
- Filtered out null or irrelevant records.
- Derive features: hour of day, day of week, peak hours.
- Remove incomplete or invalid transactions.
- Create aggregate groupings by corridor, stop, and time.

### 4. **Exploratory Data Analysis (EDA)**
- Compare route usage, peak times, revenue per corridor.
- Visualizations: bar charts, line plots, heatmaps, pie charts.
- Map busiest corridors and stops using Leaflet with stop geolocation.

### 5. **Insight Extraction**
- Correlate passenger volume with time and corridor.
- Highlight patterns for demographic-based targeting.
- Determine the most overloaded and underutilized routes.



## AI Support: IBM Granite-3.3-8B-Instruct

This project integrates **IBM’s Granite-3.3-8B-Instruct**, a powerful instruction-tuned LLM featuring:

- **8 billion parameters**, with a **128K token context window**
- Advanced **chain-of-thought reasoning** and **instruction-following**
- Pre-trained on diverse tasks: summarization, classification, code generation, RAG, question-answering
- Supports **Fill-in-the-Middle (FIM)** for code completion and structured reasoning using `<think></think>` tags

Despite its efficiency, users must remain critical of AI-generated outputs—validating results, refining prompts, and providing clearer examples when needed.

  * Auto-generation of insights
  * Data storytelling support
  * Fast identification of key trends via conversational interface

This integration enables users to interact with the dataset more intuitively and extract insights with minimal manual exploration.


### Limitations:

On large datasets or extended executions, the model occasionally runs into resource limitations.

For instance, the following error was encountered during processing:

```python
ModelError: Prediction failed for an unknown reason. It might have run out of memory? (exitcode -9)
```

This highlights that while AI assistance is powerful, it still requires awareness of underlying system constraints—especially when handling large-scale data in hosted environments.



## Insights & Findings

Based on the initial analysis, several actionable insights and recommendations have emerged to improve the operational efficiency and user experience of the TransJakarta network:

### 1. Prioritize High-Frequency Services on Key Corridors

Corridors such as **Matraman Baru – Ancol**, **Blok M – Kota**, and **Pulo Gadung – Monas** consistently show high ridership. Increasing service frequency on these routes can help:

* Accommodate high passenger demand
* Reduce waiting times
* Minimize overcrowding during peak periods

### 2. Optimize Scheduling and Fleet Deployment During Peak Hours

Passenger volume spikes during **5–8 AM** and **4–6 PM**, indicating the need for dynamic scheduling and real-time fleet optimization. Strategic measures include:

* Deploying more buses on high-demand routes during these hours
* Using demand forecasting to reduce idle fleet time and operational inefficiencies
* Enhancing ride comfort by mitigating congestion during rush hours

### 3. Leverage Demographic Segmentation for Targeted Marketing

Utilizing passenger demographic data enables personalized engagement and demand shaping through:

* **Student and senior discounts**
* **Bank and e-wallet promotions**
* **Time-based fare adjustments** to encourage off-peak ridership
* Cross-subsidization strategies to balance traffic flow and optimize resource usage

## Documentations

