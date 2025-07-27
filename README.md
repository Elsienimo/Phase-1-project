# Aircraft Purchase Data Analysis for Commercial and Private Aviation  

## Project Overview  
This project analyzes **aviation accident data (2013–2023)** from the **National Transportation Safety Board (NTSB)** to help a company make **data-driven decisions** on purchasing aircraft for both **commercial airline operations** and **private charter/training services**.  

The analysis evaluates **safety, fatality rates, and operational risks** of different aircraft models to recommend the best options for the company’s entry into the aviation industry.

---

## Objectives  
- **Identify the safest aircraft models** for commercial and private operations.  
- **Analyze accident trends** by year, flight phase, weather conditions, and purpose of flight.  
- **Provide actionable business recommendations** for aircraft acquisition or leasing.  
- Support the company’s **market entry strategy** into aviation through **data-driven insights**.

---

## Dataset  
- **Source:** National Transportation Safety Board (NTSB) Aviation Accident Database  
- **Time Frame Used:** **2013–2023**  
- **Key Columns:**  
  - `event_date` – Date of the aviation event  
  - `make`, `model` – Aircraft manufacturer and model  
  - `injury_severity`, `total_fatal_injuries` – Safety indicators  
  - `broad_phase_of_flight` – Phase of flight during accident  
  - `weather_condition` – VMC (Visual) or IMC (Instrument)  
  - `purpose_of_flight` – Commercial, Personal, Training, etc.

---

## Data Cleaning & Preparation  
Standardized date format and extracted **year**  
Replaced missing values (`weather_condition`, `broad_phase_of_flight`) with `"Unknown"`  
Created a **fatal accident indicator** (`1 = fatal, 0 = non-fatal`)  
Filtered to only include aircraft with **30+ accidents** for reliable statistics

---

## Analysis Performed  
### **1. Safety by Aircraft Model**  
- Grouped by `make` and `model` to calculate:  
  - Total accidents  
  - Fatal accidents  
  - Fatal accident rate (%)  

### **2. Accident Trends (2013–2023)**  
- Accidents over time by **purpose of flight**  
- Accidents by **broad phase of flight** (takeoff, cruise, landing, etc.)  
- Accidents by **weather condition**  

### **3. Business Recommendations**  
- Which aircraft to buy/lease  
- Whether to start with private or commercial operations  
- Risk and financial considerations  

---

## Key Insights & Recommendations  
**Commercial Operations:**  
The **Airbus A320** and **Boeing 737** are the safest and most reliable commercial aircraft, making them ideal for regional and domestic operations.  

**Private/Training Operations:**  
The **Piper PA-25** (and similar Cessna models) are cost-effective and ideal for private charters and pilot training.  

**Financial Strategy:**  
Start with **leasing aircraft** for a trial period to reduce financial risk before committing to full purchase.  

**Business Growth:**  
Begin with **private charter/training services**, then gradually expand to **regional commercial flights** once demand is established.

---

## Visualizations  
Visualizations generated using **Matplotlib & Seaborn** include:  
- Accident trends over time (**line charts**)  
- Safest aircraft by fatal accident rate (**bar charts**)  
- Accidents by weather condition and flight phase (**bar charts**)  

## Tableau Dashboard
<img width="1366" height="768" alt="Tableau dashboard" src="https://github.com/user-attachments/assets/c9d295c6-9a3b-45d2-8566-7d078426fe8e" />
<img width="1366" height="768" alt="Tableau interactive dashboard" src="https://github.com/user-attachments/assets/8d417b33-817a-4fd6-8371-1b450bb39141" />


