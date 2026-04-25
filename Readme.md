# 🇮🇳 India CII — Cyber Incidents Dashboard

An automated Cyber Threat Intelligence (CTI) tool designed to monitor and visualize cyber threats against India's Critical Information Infrastructure (CII). This project processes raw incident data, performs sector-based inference, and generates an interactive 2x2 analytical dashboard.

Dashboard Preview @Dashboard.png

## 🚀 Features

* **Automated Sector Inference:** Uses regex-based logic to categorize incidents into Banking, Telecom, Gov/PSU, Defence, and more.
* **Severity Scoring:** Calculates and visualizes "Attack Probability" to help prioritize threats.
* **Interactive 2x2 Dashboard:**
    * **Volume Analysis:** Horizontal bar chart of incident counts per sector.
    * **Severity Analysis:** Comparison of average attack probabilities.
    * **Temporal Heatmap:** Date vs. Sector grid with a dynamic severity scale.
    * **Bubble Plot:** Correlates incident volume with average severity for high-level risk assessment.
* **Client-Side Filtering:** Real-time filtering by sector, date, search terms, and probability thresholds without needing a backend server.

## 🛠️ Tech Stack

* **Language:** Python 3.x
* **Data Processing:** Pandas
* **Visualization:** Plotly.js (via Python-generated HTML)
* **Styling:** CSS3 & HTML5

## 📁 Project Structure

```text
india-cti-dashboard/
├── data/
│   └── incidents_latest.csv      # Source dataset (CSV format)
├── src/
│   └── main.py                   # Main Python processing script
├── output/
│   └── cti_dashboard_2x2.html                # The generated interactive dashboard
├── requirements.txt              # Python dependencies
└── README.md                     # Project documentation

🚥 Quick Start
    1. Clone the repository:
    git clone [https://github.com/YOUR_USERNAME/india-cti-dashboard.git](https://github.com/YOUR_USERNAME/india-cti-dashboard.git)
    cd india-cti-dashboard

    2. Install dependencies:
    pip install -r requirements.txt

    3. Run the generator:
    Place your incident CSV in the data/ folder and run:
    python src/dashboard_gen.py

    4. View the results:
    Open output/index.html in any modern web browser.

📊 Dashboard Insights
    The dashboard is structured into a 2x2 grid for maximum clarity:

    1. Top Left: Which sectors are being targeted the most?
    2. Top Right: Which sectors are facing the most sophisticated/high-probability attacks?
    3. Bottom Left: When did specific sectors see spikes in activity? (Heatmap)
    4. Bottom Right: The "Risk Quadrant" — identifying high-volume, high-severity hotspots.

⚖️ License
    This project is licensed under the MIT License - see the LICENSE file for details.

Maintained by: Stellar2705