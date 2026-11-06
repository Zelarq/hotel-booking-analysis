# 🏨 Hotel Booking Demand & Cancellation Exploratory Data Analysis

A comprehensive exploratory data analysis of hotel booking demand, guest behavior, cancellation patterns, and revenue optimization metrics across City and Resort hotels.

---

## 📌 Project Overview

The hospitality industry relies on accurate demand forecasting and cancellation risk management to optimize pricing strategies and room occupancy. This project analyzes real-world hotel booking datasets containing over 119,000 reservations to uncover the core drivers of cancellations, lead-time dynamics, customer segmentation profiles, and pricing fluctuations (Average Daily Rate — ADR).

---

## 📊 Dataset Overview

The dataset (`hotel_bookings.csv`) includes 32 columns capturing operational, seasonal, and guest metrics:

* **Property Information:** Hotel Type (`City Hotel` vs. `Resort Hotel`).
* **Booking Dynamics:** `is_canceled`, `lead_time` (days between booking and arrival), `arrival_date_year`, `arrival_date_month`, `arrival_date_week_number`.
* **Stay Characteristics:** `stays_in_weekend_nights`, `stays_in_week_nights`, `adults`, `children`, `babies`, `meal` options.
* **Customer Profile & Distribution:** `country` of origin, `market_segment`, `distribution_channel`, `is_repeated_guest`.
* **Financial & Booking Policies:** `deposit_type` (No Deposit, Non Refund, Refundable), `customer_type` (Transient, Contract, Group, Transient-Party), `average_daily_rate` (ADR), `total_of_special_requests`.

---

## 🔍 Key Findings & Business Insights

1. **Hotel Volume & Revenue Dynamics:**
   * **City Hotels** register significantly higher total booking volumes compared to Resort Hotels.
   * **Average Daily Rate (ADR)** exhibits sharp seasonal swings in Resort Hotels, peaking heavily during peak summer months (July–August), whereas City Hotels maintain more stable pricing across the year.

2. **Lead Time & Cancellation Propensity:**
   * Lead time exhibits a strong right-skewed distribution spanning up to 600+ days.
   * Bookings with extended lead times demonstrate markedly higher cancellation rates, highlighting the need for dynamic deposit requirements on long-horizon reservations.

3. **Booking Policy & Deposit Anomalies:**
   * Counterintuitively, bookings flagged under **Non-Refundable deposits** show high cancellation concentrations in historical records, primarily driven by wholesale and group reservations made through travel agents.

4. **Customer Loyalty & Special Requests:**
   * Repeat guests demonstrate high retention, significantly lower cancellation probability, and predictable special service requests compared to first-time travelers.

5. **Customer Segmentation & Outlier Control:**
   * FacetGrid boxplot analysis (filtering ADR outliers > 1,000) highlights distinct willingness-to-pay differences across Transient, Contract, and Group customer types.

---

## 📈 Visualizations in the Notebook

* **Property Comparisons:** Count plots of bookings and bar plots of Average Daily Rate by hotel property.
* **Lead Time Distribution:** Histogram with custom 30-day interval binning.
* **Customer Proportions:** Pie chart illustrating market segment proportions.
* **Cancellation Policies:** Grouped count plots evaluating cancellations across deposit policies and hotel types.
* **Service Analysis:** Bar plots tracking average special requests between new vs. repeated guests.
* **Seasonal Trends:** Line plot tracking ADR and booking volume trajectories month-over-month.
* **Facet Grid Box Plots:** Multi-facet comparison of customer types and room rates across hotel categories.
* **Correlation Heatmap:** Correlation matrix evaluating numerical variables against cancellation and lead times.

---

## 🛠️ Tech Stack

* **Language:** Python 3.x
* **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `jupyter`
* **Dataset:** `hotel_bookings.csv`

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/Zelarq/hotel-booking-analysis.git
cd hotel-booking-analysis
```

### 2. Set Up Virtual Environment
```bash
python -m venv venv
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook
```bash
jupyter notebook hotelbooking_project.ipynb
```

---

## 👤 Author

* **Sayanth N K**
* GitHub: [@Zelarq](https://github.com/Zelarq)
* Email: [sayanthnk32@gmail.com](mailto:sayanthnk32@gmail.com)

