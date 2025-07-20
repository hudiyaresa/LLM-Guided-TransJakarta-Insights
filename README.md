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

There are actually still many things that can be explored with the following data. For an initial analysis, here are some key insights and recommendations that can be concluded

### 1. Boost High-Frequency Services on Top Corridors
- Routes such as **Matraman Baru – Ancol**, **Blok M – Kota**, and **Pulo Gadung – Monas** have consistently high passenger volumes.
- These corridors would benefit from more frequent services to accommodate demand and reduce overcrowding.

### 2. Optimize Scheduling and Fleet Deployment During Peak Hours
- Peak passenger activity occurs during **5–8 AM** and **4–6 PM**.
- Buses should be allocated in higher frequency during these hours, especially on busy routes.
- For passengers, this reduces waiting time and improves overall ride comfort.

### 3. Use Demographic Targeting in Marketing Strategies
- Demographic segmentation (students, employees, elderly) can be applied to design:
  - **Student discounts**
  - **Bank or mobile payment promos**
  - **Time-based fare discounts** for incentivizing travel during off-peak hours
- These measures can help balance demand across time and routes while encouraging higher ridership.

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