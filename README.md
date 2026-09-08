# 🎧 Global Music Listener Preferences

Exploratory data analysis of global music streaming behavior, built with Python and visualized in an interactive Power BI dashboard.

**Stack:** Python (Pandas, Seaborn, Matplotlib) → Power BI

---

## 📌 Project Overview

This project explores how age, subscription type, platform, and country shape music listening behavior. It analyzes a global streaming dataset to answer questions like *who listens to what, when, and how much* — then turns those findings into an interactive dashboard.

**Key questions explored:**
1. What are the most popular music streaming platforms?
2. How does age impact music preferences?
3. What are the most streamed genres and artists?
4. How do free vs. premium users differ in streaming behavior?
5. What time of day do users stream music the most?
6. Are there regional trends in music streaming preferences?

---

## 🗂️ Repository Structure

| File | Description |
|---|---|
| `global__music_streaming_listener_preferences.py` | Python script that loads, cleans, and explores the dataset — includes boxplots, value counts, crosstabs, and grouped comparisons answering the key questions above. |
| `Global_Music_Streaming_Listener_Preferences.csv` | The raw dataset used for analysis. |
| `Global_Music_Streaming_Listener_Preferences.pbix` | Power BI dashboard built on the dataset. |
| `LICENSE` | MIT License. |

---

## 📁 Dataset Summary

- **Format:** CSV
- **Key columns:**
  - `User_ID` — unique listener identifier
  - `Age`, `Country` — demographic and geographic attributes
  - `Streaming Platform` — e.g. Spotify, Apple Music, Amazon Music
  - `Top Genre`, `Most Played Artist` — listening preferences
  - `Subscription Type` — Free vs. Premium
  - `Minutes Streamed Per Day` — daily listening volume
  - `Number of Songs Liked`, `Discover Weekly Engagement (%)`, `Repeat Song Rate (%)` — engagement metrics
  - `Listening Time (Morning/Afternoon/Night)` — time-of-day habit

---

## 🧹 Analysis Workflow (Python)

The script:
- Loads the dataset and checks shape, types, nulls, and duplicates
- Uses boxplots to inspect the distribution of numeric fields (`Age`, `Minutes Streamed Per Day`, `Number of Songs Liked`, `Discover Weekly Engagement (%)`, `Repeat Song Rate (%)`)
- Buckets listeners into age groups (`<18`, `18-30`, `31-45`, `46-60`) and cross-tabulates against `Top Genre`
- Ranks artists and genres by total minutes streamed
- Compares Free vs. Premium subscribers across streaming minutes, songs liked, discovery engagement, and repeat rate
- Breaks down listening activity by time of day and by country

**Run it:**
```bash
pip install pandas numpy matplotlib seaborn
python global__music_streaming_listener_preferences.py
```
> Note: the script currently reads from `/content/Global_Music_Streaming_Listener_Preferences.csv` (a Colab path). Update this to the local CSV path before running outside Colab.

---

## 📊 Dashboard (Power BI)

`Global_Music_Streaming_Listener_Preferences.pbix` turns the analysis into an interactive dashboard for exploring listener behavior by platform, genre, age group, and country.

**To view it:** open the file in [Power BI Desktop](https://www.microsoft.com/en-us/power-platform/products/power-bi/desktop) (free).

---

## 📈 Key Findings

- 🎧 **Amazon Music** is the most preferred streaming platform in the dataset; **Apple Music** is the least preferred.
- 🎸 **Rock** is the most-streamed genre by total minutes.
- 🌙 **Night** is the most popular time of day for listening.
- 💳 Free and Premium users show **no significant difference** in average discovery engagement or repeat listening behavior.
- 🌍 Country-level differences in genre preference exist but are **not strongly pronounced**.

---

## 🚀 Getting Started

```bash
git clone https://github.com/rawat2003raju-lab/Global-listener-music-preferences.git
cd Global-listener-music-preferences
pip install pandas numpy matplotlib seaborn
```

1. Run the Python script to reproduce the exploratory analysis.
2. Open the `.pbix` file in Power BI Desktop to explore the dashboard.

---

## 🛠️ Tech Stack

- **Python** — Pandas, NumPy, Seaborn, Matplotlib
- **Power BI** — interactive dashboarding

---

## 👤 Author

**Raju Rawat**
- GitHub: [@rawat2003raju-lab](https://github.com/rawat2003raju-lab)
- LinkedIn: [raju-rawat](https://www.linkedin.com/in/raju-rawat-4a6233251/)

---

## 📄 License

Licensed under the [MIT License](LICENSE).
