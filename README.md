# Data Analysis Projects (DAP)
This repository contains data analysis and predictive modeling projects, showcasing data preparation, exploratory analysis, grouping/aggregation, and classification modeling.

---

## 📂 Repository Structure
```text
├───car-emissions
│       project_dap_phase_1.ipynb       # Data cleaning, normalization, and merging
│       project_dap_phase_2.ipynb       # Predictive modeling and classification
│
└───rainfall
        Assignment3_SECP3233.ipynb      # Exploration, grouping, and visualization
```

---

## 🚗 Project 1: Car Registrations & CO₂ Emissions Analysis
### Course: SECP3223

This project analyzes car registration records in Malaysia to study and predict CO₂ emissions across different states and fuel types.

#### Phase 1: Data Preparation & Cleaning
- **Datasets**: Combined car registration logs (`cars_2025.csv`) with emission profiles (`FuelConsumption.csv`).
- **Pipeline**:
  - Sanitized and standardized key values (converting maker/model strings to uppercase and stripping whitespaces).
  - Merged datasets on standardized keys.
  - Handled missing data and filtered out rows lacking CO₂ data.
  - Formulated pivot tables analyzing average CO₂ emissions by state and fuel type (e.g., diesel, petrol, hybrid).

#### Phase 2: Predictive Modeling
- Categorized CO₂ emissions into **Low**, **Medium**, and **High** risk levels.
- Applied `OneHotEncoder` to encode categorical location features.
- Partitioned dataset into 80% training and 20% testing sets.
- Trained a **K-Nearest Neighbors (KNN)** classifier to predict emissions categories based on geographical and maker variables.

---

## 🌧️ Project 2: Rainfall Data Analysis
### Course: SECP3233

An exploratory study investigating monthly rainfall volumes, temperatures, and weather station demographics (Urban vs. Rural) across different regions.

#### Key Implementations:
- **Data Exploration**: Handled data loading, null values, and summary statistics.
- **Grouping & Aggregation**:
  - Station-specific aggregations (total rainfall, average rainy days, and average temperatures).
  - Regional & Urban/Rural pivot analysis.
  - Identified months and regions with peak rainfall profiles (e.g., peak levels in the West region during September).
- **Data Visualization**: Plotted detailed bar charts displaying total rainfall by region, color-coded by Urban/Rural splits using `matplotlib` and `seaborn`.


---

## 💭 Course Reflection
Using Python to perform exploratory data analysis and visual storyboarding here was my first look into analytics. It taught me how to handle missing values, decode messy encodings, and present clear visual arguments to stakeholders.
