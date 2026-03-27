# Houston Event Market Forecaster (March 2026) 🚀

A Python-based volatility tracker monitoring the "Get-In" prices for major Houston events. This project identifies buying opportunities and analyzes market shifts by comparing daily baseline prices against real-world game outcomes.

## 📊 Current Monitoring (7-Event Array)
* **NCAA Sweet 16 (3/26):** Tracked the "Cougar Tax" peak at **$537**. (Closed)
* **NCAA Elite 8 (3/28):** Real-time analysis of the "Loss-Scenario" price collapse.
* **Astros Opening Day (3/26):** Monitored price decay leading to first pitch. (Closed)
* **Astros Game 2 (3/27):** Tracking the Friday "Fireworks Night" floor of **$36.00**.
* **Houston Open (3/26-3/29):** Monitoring the weekend surge for PGA Tour rounds.
* **Rockets vs. Knicks (3/31):** Mid-range tracking for NBA regular season demand.
* **Peso Pluma (4/02):** Long-term trend analysis for high-demand concert inventory.

## 🗓️ Run Schedule
To maintain a consistent data visualization, the tracker follows a 12-hour synchronized update:
* **9:00 AM** - Morning Baseline (Market Open)
* **6:00 PM** - Evening Close (Pre-Game/Post-Event Volatility)

## 🔍 Data Methodology
Data is manually aggregated from **SeatGeek** (Get-In price including estimated fees) to track the absolute lowest entry point for fans. By using a manual pull, the project avoids "sponsored" or "featured" listing bias.

## 🔮 Prediction Engine & Post-Mortem
The forecast originally utilized a "Win-Scenario" model, where a home team victory typically spikes subsequent session prices to ~85% of the previous peak.

**Update (March 27):** Because Houston lost in the Sweet 16 on March 26, the expected Elite 8 price surge failed to materialize. Instead of climbing toward the predicted **$450+** mark, prices stabilized and began to decay into the **$220** range. This proves that **Hyper-Local Demand** is the primary driver of volatility in tournament markets—once the "Home Team" is eliminated, the secondary market supply instantly outpaces demand.

## 🛠️ Tech Stack
* **Python 3.x**
* **Pandas:** Data manipulation and timeframe management.
* **Matplotlib:** Data visualization featuring high-contrast reference lines (Cyan/Red) and **enforced $50-increment Y-axis scaling** for professional granularity.