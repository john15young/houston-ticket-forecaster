# Houston Event Market Forecaster (March 2026) 🚀

A Python-based volatility tracker monitoring "Get-In" floor prices for major Houston events. This project identifies buying opportunities and analyzes market shifts by comparing daily baseline prices against real-world outcomes and supply-demand cycles.

## 📊 Monitoring Array (Active & Historical)
* **NCAA Sweet 16 (3/26):** Tracked the "Cougar Tax" peak at **$537**. (Final)
* **NCAA Elite 8 (3/28):** Real-time analysis of the "Loss-Scenario" price collapse. Floor stabilized at **$81.00**.
* **Houston Open (3/26-3/29):** Weekend surge tracking for PGA Tour; currently **$92.00**.
* **J. Cole: The Fall-Off Tour (9/16):** Long-term anchor tracking for high-demand stadium tours; floor at **$97.00**.
* **Peso Pluma (4/02):** High-demand concert inventory analysis; floor at **$175.00**.
* **Astros Game 2 (3/27):** Friday "Fireworks Night" floor tracking—dropped to **$28.00**.

## 📈 Technical Methodology: Smoothing Volatility
To separate market "noise" from actual trends, this version implements a **3-Day Simple Moving Average (SMA)** for high-volatility events. 

* **Why SMA?** In ticket markets, a single cheap "outlier" listing can temporarily skew the floor price. The SMA provides a "Signal" that represents the true market momentum over a 72-hour window.
* **The "Crash" Insight:** While the **Elite 8** raw price hit a low of $57, the SMA reveals the market "weight" remained higher, signaling a potential dead-cat bounce that eventually brought the price back to $81.

## 🔍 Data Integrity
Data is manually aggregated from **SeatGeek** (Get-In price including fees) to ensure a 100% human-verified baseline, avoiding "sponsored" listing bias common in API-driven scrapers.

## 🛠️ Tech Stack
* **Python 3.x**
* **Pandas:** Data manipulation and SMA rolling-window calculations.
* **Matplotlib:** Advanced visualization with dual-line (Raw vs. SMA) mapping.