# Houston Event Market Forecaster (March 2026) 🚀

A Python-based volatility tracker monitoring "Get-In" floor prices for major Houston events. This project identifies buying opportunities and analyzes market shifts by comparing daily baseline prices against real-world outcomes and supply-demand cycles.

## 📊 Monitoring Array (March/April 2026)
* **NCAA Sweet 16 (3/26):** Tracked the "Cougar Tax" peak at **$537**. (Final)
* **NCAA Elite 8 (3/28):** Real-time analysis of the "Loss-Scenario" price collapse. Floor stabilized at **$81.00**.
* **Houston Open (3/26-3/29):** Weekend surge tracking for PGA Tour; currently **$92.00**.
* **Peso Pluma (4/02):** High-demand concert inventory analysis; floor at **$175.00**.
* **Astros Opening Day (3/26):** Monitored price decay leading to first pitch. (Final)
* **Astros Game 2 (3/27):** Friday "Fireworks Night" floor tracking—dropped to **$28.00**.
* **Rockets vs. Knicks (3/31):** Mid-range tracking for NBA regular season demand; stable at **$31.00**.

## 📈 Technical Methodology: Smoothing Volatility
To separate market "noise" from actual trends, this version implements a **3-Day Simple Moving Average (SMA)** for high-volatility events. 

* **Why SMA?** In ticket markets, a single cheap "outlier" listing can temporarily skew the floor price. The SMA provides a "Signal" that represents the true market momentum over a 72-hour window.
* **The "Crash" Insight:** While the **Elite 8** raw price hit a low of **$57.00**, the SMA revealed the market "weight" remained higher, correctly signaling the "dead-cat bounce" back to **$81.00**.

## 🎨 Visual Logic & Granularity
The visualization engine is configured for professional-grade market analysis:
* **High-Contrast Mapping:** Key events (NCAA/PGA) use bold **linewidth=4** to separate primary analysis from background "noise."
* **Z-Order Layering:** Critical trendlines are rendered on the top layer to ensure visibility during high-overlap periods.
* **Granular Y-Axis:** Scaling is enforced at **$50 increments** using `MultipleLocator` to provide better technical resolution than standard $100 interval plotting.

## 🔍 Data Integrity
Data is manually aggregated from **SeatGeek** (Get-In price including fees) to ensure a 100% human-verified baseline, avoiding "sponsored" listing bias common in API-driven scrapers.

## 🛠️ Tech Stack
* **Python 3.x**
* **Pandas:** Data manipulation and SMA rolling-window calculations.
* **Matplotlib:** Advanced visualization featuring dual-line (Raw vs. SMA) mapping and ticker-based axis control.