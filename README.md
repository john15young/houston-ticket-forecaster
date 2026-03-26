# Houston Event Ticket Price Forecast (March 2026)

A Python-based volatility tracker monitoring the "Get-In" prices for major Houston events. This project identifies buying opportunities and predicts market spikes leading up to game day.

## 📈 Current Monitoring
* **NCAA Sweet 16 (3/26):** Tracking tonight's Session 1 "Cougar Tax."
* **NCAA Elite 8 (3/28):** Modeling the "Win-Scenario" spike for Session 2.
* **Astros Opening Day (3/26):** Monitoring price decay as first pitch approaches.
* **Rockets vs. Knicks (3/31):** Mid-range tracking for NBA regular season demand.
* **Peso Pluma (4/02):** Long-term trend analysis for high-demand concerts.

## 🗓️ Run Schedule
To capture the most accurate volatility, this notebook is updated at:
* **9:00 AM** - Morning Baseline
* **1:00 PM** - Mid-Day Trend Check
* **6:00 PM** - Final Pre-Game Volatility

## 🔍 Data Methodology
Data is manually aggregated from **SeatGeek** (Get-In price including estimated fees) to track the lowest entry point for fans. 

## 🔮 Prediction Engine
The forecast includes a win-scenario model. If the home team wins an elimination round, the subsequent session is modeled at ~85% of the previous session's peak price.