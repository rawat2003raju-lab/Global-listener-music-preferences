# Clone the Repository:
git clone [https://github.com/your-username/global-music-listener-preferences.git](https://github.com/your-username/global-music-listener-preferences.git)
cd global-music-listener-preferences

# jupyter notebook notebooks/EDA_Music_Preferences.ipynb

#Contact & Connect
#If you have any questions, feedback, or collaboration ideas, feel free to reach out!

👤 Name:[Raju Rawat]

💼 LinkedIn: https://www.linkedin.com/in/raju-rawat-4a6233251/

💻 GitHub Portfolio: https://github.com/rawat2003raju-lab




# 🎧 Global Music Listener Preferences — End-to-End Data Analytics Project

## 📌 Project Overview
The **Global Music Listener Preferences** project analyzes user behavior, streaming patterns, genre trends, and demographic preferences across global music platforms. 

The objective of this project is to build a complete end-to-end data analytics pipeline—transforming raw streaming dataset into actionable business insights using **Python (Pandas, Seaborn, Matplotlib)**, **SQL**, and **Power BI**.

---

## 📁 Dataset Summary
* **Dataset Name:** Global Music Listener Preferences
* **Format:** CSV File
* **Key Columns:**
  * `User_ID`: Unique listener identifier
  * `Age` & `Gender`: Demographic attributes
  * `Country` / `Region`: Geographical location
  * `Primary_Genre`: Preferred music genre (*Pop, Rock, Hip-Hop, Classical, EDM, Jazz, Latin*)
  * `Streaming_Hours_Per_Day`: Daily music consumption duration
  * `Preferred_Platform`: Streaming service (*Spotify, Apple Music, YouTube Music, Amazon Music*)
  * `Subscription_Type`: Free vs. Premium plan
  * `Listening_Device`: Device type (*Mobile, Desktop, Smart Speaker*)

---

## 🛠️ Tools & Technologies
| Stage | Tool / Library | Key Application |
| :--- | :--- | :--- |
| **Data Ingestion & Cleaning** | Python, Pandas, NumPy | Missing value imputation, deduplication, feature engineering |
| **Exploratory Data Analysis** | Seaborn, Matplotlib | Visualizing distributions, correlation heatmaps, genre trends |
| **Database & Analytics** | PostgreSQL / MySQL / SQL Server | Business logic queries, aggregations, cohort segmentation |
| **Interactive Dashboard** | Power BI | DAX measures, cross-filtering, dynamic reports & KPIs |

---

## ⚙️ Project Pipeline & Execution

### 1️⃣ Data Cleaning & Preprocessing (Python)
* Loaded raw dataset into Pandas DataFrames.
* Handled missing records in numerical columns (`Streaming_Hours_Per_Day`) using median values.
* Removed duplicate listener IDs and corrected inconsistent categorical text values.
* Feature engineered `Age_Group` buckets (*18–24*, *25–34*, *35–49*, *50+*).

### 2️⃣ Exploratory Data Analysis (EDA)
Using **Seaborn** and **Matplotlib**, key visualizations were generated:
* **Genre Popularity:** Bar plots identifying top-streamed music genres globally.
* **Streaming Hours by Subscription:** Box plots comparing daily usage between Free and Premium tiers.
* **Demographic Breakdown:** Seaborn heatmaps displaying age and genre cross-tabulations.
* **Platform Dominance:** Donut charts illustrating market share across devices and apps.

### 3️⃣ SQL Database Queries
Cleaned data was imported into the relational database to execute complex analytical queries:
* **Top Genres per Region:** Calculated leading genres by total listener count across continents.
* **User Retention & Engagement:** Computed average daily listening hours grouped by subscription tier and primary device.
* **High-Value Customer Profiling:** Identified demographical groups driving premium conversions.

### 4️⃣ Power BI Dashboard
Built an interactive dashboard featuring:
* **KPI Cards:** Total Active Users, Average Daily Streaming Hours, Premium Subscriber Ratio.
* **Geographical Map:** Regional engagement distribution across countries.
* **Interactive Slicers:** Dynamic filtering by Country, Age Group, Platform, and Subscription Status.

---

## 📊 Key Results & Insights
* 🎵 **Top Genres:** **Pop** and **Hip-Hop** dominate total stream volume globally, while **Classical** and **Jazz** exhibit higher average session lengths among listeners aged 35+.
* 💳 **Subscription Impact:** Premium users average **1.8x more streaming hours per day** compared to free-tier users.
* 📱 **Device Usage:** **Mobile devices** account for **>70%** of total daily streaming hours, highlighting a mobile-first user base.
* 🌍 **Regional Growth:** **Latin music** shows the highest rate of year-over-year listener growth in North American and European markets.

---

## 💻 How to Run This Project

### Prerequisites
Install Python and required libraries:
```bash
pip install pandas numpy matplotlib seaborn
