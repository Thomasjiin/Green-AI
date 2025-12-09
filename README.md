# Green-AI: Global Deforestation Analysis & Forecasting

This project analyzes global and regional deforestation patterns using open-source datasets from Our World in Data and applies machine learning and forecasting models to understand trends and potential future scenarios.
The work includes exploratory data analysis, interactive visualizations, regional comparisons, feature-driven modeling, and forecasting up to 2030.

Authors: ZENG Yijia, GEORGES Nathan, GAUTHÉ Thibault, JIN Thomas, ZHOU JINXIN

### 1. Project Overview

Deforestation remains one of the most critical environmental challenges, impacting biodiversity, carbon storage, and climate regulation. This project uses historical global datasets to:

Explore long-term and regional deforestation trends

Identify key factors linked to forest loss

Predict future deforestation using AI models

Visualize patterns across countries and time

Discuss uncertainties and ethical aspects of forecasting environmental risks

### 2. Key Features of the Project
2.1 Global Trend Analysis

Visualization of the historical global deforestation rate (in million hectares per year).

Trend interpretation showing long-term reduction in forest loss since the early 2000s.

2.2 Regional Trend Comparison

A comparison of World vs Asia, Africa, South America, North America, Europe reveals how different regions contribute to global forest loss.
South America and Africa dominate total losses, while Asia shows a gradual decline and Europe remains stable.

2.3 Interactive Visualizations

The notebook includes multiple interactive Plotly visualizations:

Global time-series trends

Top deforesting countries

Animated choropleth maps showing change over time

Forest cover distribution by country

Net forest change and transition matrix plots

These help uncover spatial and temporal patterns in a clear and intuitive way.

### 3. AI-Driven Modeling
3.1 Linear Regression Forecast (Global)

A simple linear model predicts a continued decline in global deforestation, projecting values around 7 M Ha/yr by 2030.

3.2 Prophet Forecast (with Uncertainty Interval)

A more modern time-series model (Prophet) is used to forecast the deforestation trajectory:

Captures general downward trend

Adds uncertainty bands (yhat_lower, yhat_upper)

Helpful for scenario-based interpretation

3.3 Multi-Feature Regression (Country-Level Drivers)

Using countries’ annual data, a Random Forest regression identifies the key predictors of deforestation:

Features used:

Annual net forest change

Forest cover share (%)

Per-capita embodied CO₂ emissions

Feature Importance Result:
Annual net forest change is the strongest predictor, while forest cover and per-capita CO₂ contribute far less.

This helps explain which variables most strongly relate to forest loss at the country-year level.

3.4 Country-Level AI Forecasts

Linear models were also fitted per country (when data available) to estimate likely net forest change by 2030, then displayed on a global choropleth map.

### 4. Data Source

All datasets come from Our World in Data – Deforestation Database:

https://ourworldindata.org/deforestation

Main tables used:

annual-deforestation.csv

forest-area-as-share-of-land-area.csv

annual-change-forest-area.csv

per-capita-co2-food-deforestation.csv

forest-transition-phase.csv

Each dataset includes country/region names, ISO codes, years, and the relevant environmental indicators.

### 5. Ethical AI & Limitations
Data limitations

Missing values, inconsistent years, and limited coverage introduce uncertainty.

Key socio-economic and policy drivers are not fully represented in the dataset.

Model limitations

Linear models assume stable trends; Prophet assumes smooth long-term patterns.

None of the models can capture sudden changes caused by policy shifts, climate events, economic crises, or illegal clearing.

Forecast uncertainty

Forecast results should be treated as scenario estimates, not exact predictions.

Ethical considerations

Misinterpreting predictions may misguide environmental policy or unfairly pressure certain countries.

Transparency in uncertainty is essential.

### 6. Conclusion

This project provides a comprehensive data-driven view of global deforestation, combining:

Clear visual evidence of long-term global decline

Strong regional contrasts

Machine learning insights into key drivers

Forecasts extending to 2030 with uncertainty

Ethical reflection on responsible AI use

The combination of historical data, modern forecasting, and feature-level interpretation offers a holistic understanding of deforestation dynamics on a global scale.