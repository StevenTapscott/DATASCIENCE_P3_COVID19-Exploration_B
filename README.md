# COVID-19 Data Exploration Across G8 Countries

## Project Overview
This project explores COVID-19 trends across G8 countries using public datasets from Our World in Data. The analysis focuses on daily confirmed cases, deaths, and vaccination rollout trends using time series analysis, rolling averages, annotated visualisations, and comparative metrics.

The objective of the project is to identify and communicate key pandemic patterns across economically developed nations with differing public health responses and vaccination strategies.

---

# Objectives
- Explore and inspect COVID-19 public health datasets
- Compare pandemic trends across G8 countries
- Visualize case, death, and vaccination trends over time
- Apply rolling averages to smooth reporting noise
- Standardize metrics per 100,000 people
- Create annotated multi-country comparison charts
- Summarize key epidemiological findings

---

# Countries Included
- United Kingdom
- United States
- Germany
- France
- Italy
- Canada
- Japan
- Russia

---

# Datasets Used

## 1. Daily COVID-19 Cases Per Million
File:

```text
daily-new-confirmed-covid-19-cases-per-million-people.csv
```

## 2. Daily COVID-19 Deaths Per Million
File:

```text
daily-new-confirmed-covid-19-deaths-per-million-people.csv
```

## 3. Daily Vaccination Rates Per Million
File:

```text
daily-share-of-the-population-receiving-a-first-covid-19-vaccine-dose.csv
```

Source:
- Our World in Data COVID-19 Dataset

---

# Technologies & Skills Used
- Python
- pandas
- matplotlib
- seaborn
- Time series analysis
- Rolling averages
- Data visualization
- Public health analytics
- Comparative analysis
- Data storytelling

---

# Data Preparation

## Dataset Inspection
Each dataset was inspected to identify:
- key variables
- data types
- missing values
- date formatting requirements

## Date Conversion
The `Day` column was converted to datetime format to support time series analysis.

```python
cases['Day'] = pd.to_datetime(cases['Day'], dayfirst=True)
```

## Standardized Metrics
Since the datasets were already normalized per million population, metrics were converted to rates per 100,000 people by dividing values by 10.

---

# Analysis Performed

## 1. Multi-Country Time Series Analysis
Line charts were created to compare:
- COVID-19 case trends
- death trends
- vaccination rollout rates

across G8 countries.

---

## 2. Rolling 7-Day Averages
Rolling averages were applied to:
- smooth reporting noise
- reduce short-term volatility
- improve trend readability

---

## 3. Annotated Visualizations
Charts were annotated with major pandemic milestones:
- WHO pandemic declaration
- vaccine rollout periods
- Omicron emergence

to improve interpretability and contextual storytelling.

---

## 4. Population-Standardized Comparisons
Death and vaccination metrics were standardized to rates per 100,000 people to support fair cross-country comparisons.

---

# Key Findings

## COVID-19 Cases
- France and the United Kingdom experienced some of the largest infection waves during the Omicron period.
- Japan maintained comparatively lower case levels during earlier phases of the pandemic but experienced delayed later waves.

---

## COVID-19 Deaths
- France and Germany recorded the highest average death rates per 100,000 among G8 countries in the analyzed period.
- Japan and Canada maintained comparatively lower mortality levels.

---

## Vaccination Rollout
- The United Kingdom and United States demonstrated strong early vaccination rollout rates.
- Japan showed a slower initial rollout followed by rapid acceleration later in 2021.
- Russia maintained comparatively lower vaccination intensity during much of the rollout period.

---

# Final Insights
The analysis suggests that although later pandemic waves produced extremely large infection surges across many G8 countries, death rates generally remained lower relative to earlier waves. This trend coincided with widespread vaccine rollout campaigns and may reflect the combined impact of vaccination, improved treatment strategies, prior immunity, and evolving public health responses.

The project also demonstrates how rolling averages and annotated visualisations can improve the communication of complex public health trends.

---

# Example Visualizations
The project includes:
- Multi-country case trend charts
- Rolling-average death trend charts
- Vaccination rollout comparisons
- Annotated pandemic timeline visualizations
- Population-standardized comparison charts

---

# Skills Demonstrated
- Exploratory Data Analysis (EDA)
- Time series analysis
- Rolling average calculations
- Comparative country analysis
- Data visualization
- Public health data interpretation
- Annotated chart design
- Analytical storytelling
- Population-standardized metrics

---

# Future Improvements
- Add interactive dashboards using Plotly or Power BI
- Incorporate hospitalization datasets
- Compare policy interventions and lockdown timing
- Add forecasting models
- Perform statistical correlation analysis between vaccination rates and mortality
