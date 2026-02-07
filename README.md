# CDC Diabetes Risk & Lifestyle Analysis
### Transforming 250k+ Health Surveys into Actionable Insights

> **"I turned 250,000 CDC health records into an interactive story about how our daily habits and backgrounds shape our health. This dashboard pinpoints exactly where lifestyle meets risk, helping us see who is most vulnerable to diabetes and how we can bridge that gap."**

---

## 📌 Project Overview
Type 2 Diabetes is a significant public health challenge, yet many cases are preventable through lifestyle intervention. This project analyzes a dataset of **253,680 survey responses** from the CDC’s 2015 Behavioral Risk Factor Surveillance System (BRFSS). 

The goal was to move beyond simple statistics and identify the specific **"Risk Intersections"** where socio-economic status, clinical markers, and lifestyle habits collide to drive diabetes prevalence.

## 🛠️ The Tech Stack
* **Excel:** Data cleaning, handling null values, and creating lookup tables to transform numeric codes (1.0, 2.0) into human-readable categories.
* **Power BI & Power Query:** Data modeling and advanced data transformation.
* **DAX (Data Analysis Expressions):** Created dynamic measures including:
    * **Diabetes Prevalence Rate:** A context-aware measure of confirmed cases vs. total population.
    * **National Average Target:** An `ALL` filtered measure used for benchmarking specific demographics.

## 📊 Key Analytical Insights

### 1. The Wealth Gap in Public Health
The analysis identified a clear inverse relationship between income and health. As household income moves from "Low" (<$25k) to "High" ($75k+), the diabetes prevalence rate drops significantly, suggesting that socio-economic status serves as a protective "buffer."

### 2. The "Lifestyle vs. Biology" Offset
A deep dive into clinical risk factors revealed that **Physical Activity** acts as a powerful moderator. Even among individuals with high blood pressure, those who are physically active show a measurably lower diabetes prevalence than those who are inactive.

### 3. The BMI "Danger Zone"
Using scatter plot clustering, the analysis pinpointed a critical risk zone: **individuals over age 45 with a BMI exceeding 30.** This demographic represents the highest density of confirmed cases and should be the primary target for preventative screening.

---

## 📈 Dashboard Features

### Page 1: Executive_Summary
A macro-view of national health trends, demographic breakdowns, and the socio-economic health gap.

<img width="1429" height="810" alt="Image" src="https://github.com/user-attachments/assets/ce937612-61d3-40cb-9fd2-03c87e14a01a" />

### Page 2: Risk Factor Explorer
An interactive "Why" page where users can use slicers (Smoker, Activity, Income) to see how the "Risk Gauge" swings compared to the national average.
![Risk_Analysis](Images/Risk_Analysis.png)


---

## 📂 Repository Structure
* **`Data/`**: Contains the raw BRFSS 2015 dataset.
* **`Dashboard/`**: The `.pbix` Power BI file containing the full data model and visuals.
* **`Images/`**: Screenshots of the dashboard for this README.

## 🚀 How to Use
1. Download the `Diabetes_Dashboard.pbix` file from the **Dashboard** folder.
2. Open the file in **Power BI Desktop**.
3. Navigate to **Page 2** and use the slicers to explore how different combinations of habits affect the overall risk needle.
