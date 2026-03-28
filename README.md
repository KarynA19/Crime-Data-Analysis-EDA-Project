# Crime-Data-Analysis-EDA-Project
Exploratory Data Analysis (EDA) on crime data in Israel (2020–2025)

# 📊 Crime Data Analysis in Israel (EDA Project)

## 📌 Overview
This project presents a comprehensive **Exploratory Data Analysis (EDA)** of crime data in Israel between **2020–2025**.  
The goal is to explore patterns, trends, and relationships across time, location, and crime categories.

The project was developed as part of the *Lab in Data Analysis* course.

---

## 📂 Dataset Description

The dataset includes:
- ~1.95 million records  
- 19 features  
- Mixed data types (categorical, numerical, temporal)

### Data Sources:
- Crime data: https://data.gov.il/he/datasets/israel-police/crime_records_data  
- Population data: https://data.gov.il/he/datasets/population_authority/residents_in_israel_by_communities_and_age_groups  

---

## 🎯 Project Objectives
- Perform full Exploratory Data Analysis (EDA)
- Clean and preprocess real-world data
- Integrate multiple datasets
- Extract meaningful insights using statistical analysis and visualization

---

## 🧹 Data Cleaning
- Removed rows with missing geographic information  
- Handled missing and inconsistent values  
- Removed duplicate and irrelevant records  
- Standardized column names  
- Converted data types (e.g., categorical, datetime)

---

## 🔄 Data Transformation
- Converted categorical variables to category type  
- Created new features (e.g., quarter of year)  
- Encoded variables where necessary  
- Normalized numerical values  

---

## 🔗 Data Integration
The crime dataset was merged with external population data (`people_per_city.csv`) in order to:
- Enable fair comparison between regions  
- Calculate normalized crime rates  

---

## 📊 Normalization
To ensure meaningful comparisons, crime counts were normalized:

**Crimes per 1,000 residents** were calculated by dividing total crimes by population size.

---

## 📈 Data Analysis & Visualization
The analysis includes:
- Distribution plots (histograms, KDE)
- Bar charts for categorical variables
- Time series analysis (2020–2025)
- Correlation heatmaps
- Aggregations using `groupby()`
- Pivot tables

### Key Visualizations:
- Top 10 most frequent crime types  
- Crime trends over time  
- Crime distribution by quarter  
- Crime rates per 1,000 residents  
- Regional comparisons  
- Heatmaps of crime categories by year  

---

## 🔍 Key Insights

### 1. Crime Distribution is Highly Uneven Across Regions
The analysis reveals significant disparities in crime rates between different regions and settlements.  
After normalization (crimes per 1,000 residents), some smaller regional councils appear to have disproportionately high crime rates.

However, this is largely due to **statistical amplification**:  
regions with small populations tend to show extreme values when normalized.

---

### 2. Population Size Strongly Affects Interpretation
A key finding is that **absolute crime counts can be misleading**.

- Large cities naturally show higher total crime counts  
- Smaller areas may appear “more dangerous” after normalization  

This highlights the importance of:
- Using both raw counts and normalized metrics  
- Interpreting normalized values with caution  

---

### 3. Dominance of Specific Crime Categories
A small number of crime categories consistently dominate the dataset across all years.

This suggests:
- Certain types of crime are structurally more common  
- Crime patterns are relatively stable over time  

---

### 4. Temporal Trends (2020–2025)
Crime trends over time show relatively stable behavior between 2020–2024.

A sharp drop is observed in 2025, which is likely due to:
- Incomplete or partially published data  

This emphasizes the importance of validating data completeness before drawing conclusions.

---

### 5. Seasonal Patterns (Quarter Analysis)
The distribution of crime across quarters indicates **moderate seasonal variation**.

While differences are not extreme, certain quarters consistently show slightly higher crime levels, suggesting:
- Possible seasonal or social influences  
- Periodic behavioral patterns  

---

### 6. Impact of Data Cleaning on Analysis Quality
Removing records with missing geographic data significantly improved:
- Data consistency  
- Reliability of regional comparisons  

This demonstrates how **data cleaning directly impacts analytical validity**.

---

### 7. Correlation Between Crime Type and Time
The heatmap analysis shows that:
- Some crime categories remain stable across years  
- Others fluctuate, indicating changing trends or reporting patterns  

---

### 8. Importance of Data Integration
Merging crime data with population data enabled:
- Meaningful comparisons between regions  
- Fair evaluation of crime intensity  

Without integration, insights would be biased toward larger populations.

---

### 9. Limitations of the Analysis
- Missing or incomplete data (especially 2025)  
- Normalization bias in small populations  
- Potential inconsistencies in reporting methods  

These limitations should be considered when interpreting results.

---

### 10. Practical Implications
The findings can be useful for:
- Policy makers (resource allocation)  
- Law enforcement (identifying high-risk areas)  
- Urban planning and public safety analysis  

---

## 🧰 Technologies Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Jupyter Notebook  

---


