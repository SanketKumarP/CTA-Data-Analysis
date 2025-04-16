# 🚇 Data-Driven Geospatial Analysis of Chicago Transit System  
*Exploring Performance and Efficiency in the CTA System*

## 📍 Overview  
This project evaluates the effectiveness of the Chicago Transit Authority (CTA) system through a comprehensive, data-driven analysis of routes and stations. We aimed to identify the busiest stations, monitor L-line ridership trends, assess the impact of disruptions, and compare actual travel wait times against scheduled ones. 

By combining **geospatial visualization**, **regression modeling**, and **exploratory data analysis (EDA)**, we offer insights that help optimize transit efficiency and improve commuter experiences.

---

## 🔍 Objectives  
- Identify the busiest routes and stations in the CTA system  
- Analyze ridership trends over time and across city neighborhoods  
- Detect delays/disruptions and compare wait times to scheduled times  
- Visualize geospatial patterns in ridership using interactive maps  
- Assess the impact of COVID-19 on public transportation usage  
- Propose service improvements and future directions using real-time data

---

## 🧪 Methodology  
1. **Data Collection:**  
   - Ridership data (daily/monthly) from the CTA portal  
   - L-station geospatial data and shape files  
   - Real-time API-based wait time data (proposed for future work)  
   - Survey data on commuter wait-time expectations  

2. **Data Preprocessing:**  
   - Cleaned and merged datasets by station ID  
   - Handled missing values and filtered for specific rail lines (e.g., Red Line)  
   - Converted coordinates for geospatial plotting  

3. **EDA & Modeling:**  
   - Analyzed patterns across weekday/weekend and seasons  
   - Applied simple linear and polynomial regression  
   - Visualized ridership trends over time and station-level heatmaps  

---

## 🌍 Geospatial Visualization  
We used the `Leaflet` package in R to:  
- Plot all “L” stations with real coordinates  
- Overlay **ridership intensity heatmaps**  
- Provide interactive, zoomable maps for station-level planning  

---

## 📈 Regression Modeling  
For predicting ridership fluctuations, we applied:
| Model Type               | R² Score | RMSE   |
|--------------------------|----------|--------|
| Simple Linear Regression | 0.1031   | 18,809 |
| Polynomial Degree 2      | 0.729    | 10,333 |
| Polynomial Degree 3      | 0.745    | 10,021 |

---

## 📦 Tools & Technologies  
- **Languages**: R, Python  
- **Libraries**: `Leaflet`, `ggplot2`, `fitdistrplus`, `plotly`, `DT`, `plyr`  
- **Software**: RStudio  
- **Data Sources**:  
   - [CTA Official Data](https://www.transitchicago.com/data/)  
   - [CTA Ridership Reports](https://www.transitchicago.com/ridership/)

---

## 🧠 Future Work  
- Integrate **real-time wait times** using the CTA API  
- Expand **bus route analysis** for a full network overview  
- Analyze **weather impact** on transit delays  
- Deploy dashboard for **public use or policy insights**

---

## 📁 Repository Structure
```
📂 Project Root
│
├── 📄 Project Report.pdf
├── 📄 Project Proposal.pdf
├── 📄 Project Presentation.pdf
├── 📁 Data (not included due to size/privacy)
├── 📂 Code
│   ├── data_preprocessing.R
│   ├── geospatial_visualization.R
│   └── regression_modeling.R
```
