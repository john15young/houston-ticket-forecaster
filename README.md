# Houston Event Market Forecaster (March 2026) 🚀

A Python-based volatility tracker monitoring the "Get-In" prices for major Houston events. This project identifies buying opportunities and analyzes market shifts by comparing daily baseline prices against real-world game outcomes and local team status.

## 📊 Current Monitoring (7-Event Array)
* **NCAA Sweet 16 (3/26):** Tracked the "Cougar Tax" peak at **$537**. (Closed)
* **NCAA Elite 8 (3/28):** Real-time analysis of the "Loss-Scenario" price collapse—currently at **$67.00**.
* **Astros Opening Day (3/26):** Monitored price decay leading to first pitch. (Closed)
* **Astros Game 2 (3/27):** Tracking the Friday "Fireworks Night" floor—dropped to **$30.00**.
* **Houston Open (3/26-3/29):** Monitoring the weekend surge for PGA Tour rounds; currently **$79.00**.
* **Rockets vs. Knicks (3/31):** Mid-range tracking for NBA regular season demand; stable at **$29.00**.
* **Peso Pluma (4/02):** Long-term trend analysis for high-demand concert inventory; floor at **$160.00**.

## 🗓️ Run Schedule
To maintain a consistent data visualization, the tracker follows a 12-hour synchronized update:
* **9:00 AM** - Morning Baseline (Market Open)
* **6:00 PM** - Evening Close (Pre-Game/Post-Event Volatility)

## 🔍 Data Methodology
Data is manually aggregated from **SeatGeek** (Get-In price including estimated fees) to track the absolute lowest entry point for fans. By using a manual pull and live screenshot verification, the project avoids "sponsored" or "featured" listing bias and ensures 100% data integrity during high-volatility windows.

## 🔮 Prediction Engine & Post-Mortem
The forecast originally utilized a "Win-Scenario" model, where a home team victory typically spikes subsequent session prices. 

**Update (March 27):** Because Houston lost in the Sweet 16 on March 26, the expected Elite 8 price surge failed to materialize. Instead of climbing toward the predicted **$450+** mark, the market experienced a catastrophic correction. 
* **Pre-Loss Baseline:** $215.00
* **Observed Floor:** **$67.00**
* **Total Volatility:** **-68.8% Decay**

This delta proves that for non-championship rounds, **Hyper-Local Demand** is the primary driver of price. Once the local draw is eliminated, secondary market supply instantly overwhelms demand, regardless of the event's national prestige.

## 🛠️ Tech Stack
* **Python 3.x**
* **Pandas:** Data manipulation and timeframe management.
* **Matplotlib:** Data visualization featuring time-series mapping, high-contrast reference lines, and **enforced $50-increment Y-axis scaling** for professional granularity.