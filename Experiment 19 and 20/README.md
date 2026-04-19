# Experiment 19 and 20
# 🦠 COVID-19 Data Analysis
A comprehensive Python-based Exploratory Data Analysis (EDA) of the global COVID-19 pandemic dataset. This project analyzes the spread of COVID-19 across countries worldwide, with a focused deep-dive into India's state-wise distribution. The analysis covers confirmed cases, deaths, recoveries, and active cases — presented through data aggregation, statistical summaries, and interactive choropleth visualizations.

# 📌 Table of Contents

Overview
Dataset
Tools & Libraries
Data Preprocessing
Analysis Workflow
Key Findings
Observations & Insights
Project Structure
How to Run
Author


# 🧭 Overview
The COVID-19 pandemic is one of the most significant global health crises in modern history. Understanding the spread and scale of the virus through data is crucial for making sense of its impact. This project performs a structured EDA on a real-world COVID-19 dataset to answer questions like:

## Which countries were hit hardest by the pandemic?
## What does the global distribution of confirmed cases look like?
## How did cases spread across Indian states?
## What is the ratio of active, recovered, and deceased cases?

The project was completed as part of an academic data analysis assignment and demonstrates practical use of Python for real-world data exploration.

# 📁 Dataset
## File: covid_19_data.csv
## Type: Time-series tabular data
## Granularity: Daily cumulative case counts per country/region and province/state

<img width="536" height="248" alt="image" src="https://github.com/user-attachments/assets/d1822d6b-0c69-4606-900c-fb115841f175" />


# 🛠️ Tools & Libraries
<img width="473" height="211" alt="image" src="https://github.com/user-attachments/assets/033d2a80-e349-4957-8760-298c63756cf1" />


# 🧹 Data Preprocessing
Before analysis, the raw dataset was cleaned and transformed through the following steps:
## Step 1 — Drop Irrelevant Columns
SNo (just a row index) and Last Update (redundant with ObservationDate) were removed to keep the data clean.
## Step 2 — Fix Data Types
The original CSV stores dates as strings and case counts as floats. These were corrected:

ObservationDate → datetime64[ns]
Confirmed, Deaths, Recovered → int64
## Step 3 — Derive Active Cases
A new column Active was engineered to represent ongoing cases:
Active = Confirmed - Recovered - Deaths
This gives a more meaningful picture of the actual burden on healthcare systems at any given point.
## Step 4 — Snapshot Filtering
For country-level and state-level comparisons, the dataset was filtered to only include rows from the latest available date, giving a current-state view rather than a cumulative historical view.

# 🔍 Analysis Workflow
## 1. Initial Exploration

Loaded the dataset and previewed the first few rows
Checked column data types and null values using .info()
Confirmed overall structure before beginning transformations

## 2. Global Latest Snapshot

Identified the maximum (most recent) ObservationDate in the dataset
Filtered the entire dataframe down to only that date's records
Determined the number of unique countries/regions covered (nunique())
Listed all countries present in the snapshot

## 3. Country-Level Aggregation

Grouped by Country/Region and summed Confirmed, Deaths, Recovered, and Active
Sorted by Confirmed (descending) to rank countries by case burden
Extracted individual rows for India, Mainland China, and US for direct comparison

## 4. India-Specific Deep Dive

Filtered the full dataset to only India records
Found India's latest observation date independently
Determined the number of unique provinces/states tracked for India
Grouped by Province/State and aggregated case counts
Sorted by Confirmed to rank Indian states
Identified the state with maximum confirmed cases programmatically

## 5. Map Visualizations

Built a global choropleth map using plotly.express to visualize the worldwide distribution of confirmed cases
Built an India state-level choropleth map using a GeoJSON file of Indian administrative boundaries


# 📊 Key Findings
🌍 Global — Top 5 Countries by Confirmed Cases
<img width="466" height="179" alt="image" src="https://github.com/user-attachments/assets/0ea10634-7e30-4abe-9b35-4a582a36f8c9" />
The United States recorded the highest number of confirmed cases globally, accounting for a significant share of total worldwide cases.
India ranked second, with nearly 28 million confirmed cases — a reflection of its large population and dense urban centers.
Brazil followed as the third most-affected country, with over 16 million confirmed cases.
Together, the top 3 countries alone account for a disproportionate share of all global cases.

🇮🇳 India — State-Level Observations

India's data was broken down across multiple provinces and states, offering a granular look at sub-national spread.
State-wise aggregation revealed significant regional disparity — a small number of high-density states accounted for the majority of India's total case count.
The state with the maximum confirmed cases was identified programmatically using idxmax() logic on the grouped dataframe.

# 📈 Active vs. Resolved Cases

The Active column (derived as Confirmed - Deaths - Recovered) provides a real-time view of unresolved cases.
For most countries in the later stages of the dataset, a large proportion of confirmed cases had moved to the "Recovered" category, indicating improving outcomes over time.


# 🔎 Observations & Insights
Geographic Concentration of Cases
The pandemic was not evenly distributed across the globe. A handful of large, densely populated countries — the US, India, and Brazil — accounted for the bulk of all recorded cases. This concentration points to the role that population density, urbanization, and healthcare infrastructure play in determining outbreak scale.
The Role of Population Size
India and the US together represent two very different contexts — the US has a far smaller population yet recorded more cases, suggesting that factors like early containment measures, testing capacity, and policy response played a bigger role than raw population size alone.
China's Relatively Low Late-Stage Numbers
Mainland China, despite being the origin of the outbreak, showed comparatively low confirmed case numbers in the latest snapshot. This is consistent with early strict lockdown measures that contained the initial spread — though it also reflects differences in reporting and testing protocols across countries.
India's Internal Disparity
Within India, confirmed cases were heavily skewed toward a few states. Densely populated and economically active states — with higher rates of interstate movement — contributed disproportionately to the national total. Smaller and more geographically isolated states showed significantly lower case counts, highlighting how connectivity and mobility are key drivers of viral spread.
Active Cases as a Real-Time Indicator
The derived Active column (Confirmed − Deaths − Recovered) is arguably more meaningful than raw confirmed counts for understanding current healthcare burden. In later phases of the dataset, many countries show declining active cases even as confirmed totals grew — reflecting the passage of time and rising recoveries rather than worsening conditions.
Data Limitations Worth Noting

## Underreporting: 
Confirmed case counts are heavily dependent on testing availability. Countries with limited testing infrastructure likely have significant undercounting.
Inconsistent Province/State data: Not all countries report sub-national breakdowns. India's state-level data is available, but many other countries only report national totals.
## Recovery reporting gaps: 
Some countries stopped reporting recovery data at certain points, which can make the Active count appear artificially inflated.
## Naming inconsistencies:
Country names like "Mainland China" vs. "China" require careful handling when matching against standard GeoJSON location names for map rendering.


## Maps:

<img width="1575" height="628" alt="image" src="https://github.com/user-attachments/assets/c0ec5058-2923-422a-a350-f7adef287026" />
<img width="801" height="311" alt="image" src="https://github.com/user-attachments/assets/d9c3a1c5-1476-47a8-816a-ff9a15b3f603" />

