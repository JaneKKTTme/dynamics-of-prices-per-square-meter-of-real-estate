# 📈 Real Estate Price Dynamics Dashboard

<div align='center'>
   <img src='assets/dashboard-demo.gif' alt='Interactive Dashboard Demo' width='800'/>
   <br>
   <em>✨ Interactive price dynamics visualization in action ✨</em>
</div>

An interactive data visualization dashboard built with Tableau Public that tracks the dynamics of square meter prices across Russian regions. Stop guessing and start analyzing where the market is heading! 📊

> *Warning:* Analyzing real estate prices can lead to an uncontrollable desire to buy an apartment or, conversely, to postpone this idea indefinitely! ⚠️

## 📑 Table of Contents
- [Description](#description)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Data Source](#data-source)
- [How to Use](#how-to-use)
- [Installation & Setup](#installation--setup)
- [Project Structure](#project-structure)
- [Data Processing](#data-processing)
- [Possible Improvements](#possible-improvements)
- [Feature Ideas](#feature-ideas)
- [License](#license)
- [Disclaimer](#disclaimer)

## <a id="description"></a> 📋 Description
This project transforms raw CSV data on real estate prices into a beautiful, interactive Tableau dashboard. It allows you to explore price trends for primary and secondary housing in different regions, filter by property class, and identify market patterns faster than a real estate agent can say "unique opportunity"! 🤖

## <a id="features"></a> ✨ Features
- **Interactive Dashboard** - Filter data by region, date, and property type with a single click
- **Price Dynamics** - Track how prices per square meter change over time
- **Market Segmentation** - Separate views for primary and secondary markets
- **Regional Comparison** - Compare price trends across 80+ Russian regions
- **Clean & Modern UI** - Full-screen embedded Tableau visualization with no distractions

## <a id="tech-stack"></a> 🛠️ Tech Stack
- **Data Processing:** Python (Pandas) + Jupyter Notebook
- **Visualization:** Tableau Public
- **Frontend:** HTML5 + CSS3 + JavaScript (Tableau Embedding API)
- **Data Format:** CSV / Parquet

## <a id="data-source"></a> 💾 Data Source
The data is sourced from **Domclick** and contains monthly average prices per square meter for apartments in Russian regions from January 2022 to September 2025. The dataset includes:
- **84 regions** of the Russian Federation
- **2 property categories** (Primary: business/economy, Secondary market)
- **45 months** of continuous data

## <a id="how-to-use"></a> 🎮 How to Use
1. **Open** the `index.html` file in your browser
2. **Wait** for the Tableau dashboard to load (it's worth it!)
3. **Interact** with the dashboard:
   - Use filters to select specific regions
   - Switch between market types
   - Hover over data points for exact values
4. **Analyze** trends and impress your colleagues with your data literacy

## <a id="installation--setup"></a> 🚀 Installation & Setup

1. **Clone or download** the project files
2. **NO dependency installation needed!** (unless you want to reprocess the data)
3. **Open** `index.html` in any modern web browser
4. **Enjoy** the view!

*To reprocess the data:*
```bash
# Only if you want to modify the original dataset
pip install pandas pyarrow
jupyter notebook preprocessing_data.ipynb
```

## <a id="project-structure"></a> 📁 Project Structure
```text
project/
├── index.html                                  # Main HTML page with embedded Tableau
├── dynamics of prices per square meter.csv     # Cleaned dataset (CSV)
├── dynamics of prices per square meter.parquet # Cleaned dataset (Parquet)
├── preprocessing_data.ipynb                    # Jupyter notebook for data cleaning
├── README.md                                   # This file (you're reading it!)
└── README.ru.md                                # Russian version of the README
```

## <a id="data-processing"></a> 🧹 Data Processing
The raw data was transformed using a Jupyter notebook (`preprocessing_data.ipynb`) to ensure quality and consistency:
- Parsed date column into year and month
- Removed generalized categories
- Dropped constant-value columns (source, freq, etc.)
- Excluded aggregated data for "Россия"
- Checked for negative values (none found!)
- Removed duplicates
- Exported to both CSV and Parquet formats

## <a id="possible-improvements"></a> 🛠️ Possible Improvements
- **Price Forecast** - Add predictive models to show where prices are heading
- **Mortgage Rate Overlay** - Correlate price changes with key interest rates
- **Animated Transitions** - Show price changes year-over-year with smooth animations
- **Downloadable Reports** - Allow users to export filtered data as PDF/Excel
- **Mobile Optimization** - Enhance the experience on smartphones and tablets
- **Additional Metrics** - Include average apartment size, total transaction volume

## <a id="feature-ideas"></a> 🔮 Feature Ideas
☠️ ***Price Alerts:*** Get notified when prices in your chosen region cross a threshold

🛡️ ***Investment Score:*** Calculate a "buy vs. wait" index based on historical trends

🌐 ***Browser Extension:*** Quick price lookup for any listing you find online

## <a id="license"></a> 📜 License
MIT License - because sharing is caring, and we care about your access to market data!

This project is provided *“as is”* - the dashboard works until something changes in Tableau, although everything has already changed... 🥀 Tableau is not available in the Russian Federation 😭

## <a id="disclaimer"></a> 🎭 Disclaimer
The author takes **NO** responsibility for:
- Real estate transactions made (or not made) based on this data
- Sudden urges to become a real estate mogul
- Arguments with family members about "the right time to buy"
- Hours spent playing with filters instead of working
- The realization that you'll never afford an apartment in Moscow

> Remember: A well-analyzed market is the first step to a well-made decision! Or at least a well-informed panic! 😎

***Happy analyzing!*** 🔗✨