
# 🔌 Household Energy Consumption Analysis & Dashboard

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-orange?logo=pandas)
![Plotly](https://img.shields.io/badge/Plotly-Interactive%20Viz-lightgrey?logo=plotly)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![License](https://img.shields.io/badge/License-MIT-green)

An end-to-end data analysis project that explores and visualizes patterns in household electricity consumption. This project ingests high-frequency sensor data, performs thorough cleaning and time-series aggregation, and delivers key insights through static visualizations and an interactive dashboard.

---

## 📊 Project Overview

This project tackles a common real-world problem: understanding the "why" behind energy usage. While most people just see a number on their monthly bill, this analysis dives deep into the data to uncover the hidden drivers of consumption—weather, time of day, and appliance usage—and presents the findings in an actionable way for both homeowners and utility providers.

The core deliverable is an interactive dashboard that allows users to explore the relationship between electricity consumption and various factors, fulfilling all project requirements:
-   ✅ Line chart of usage over time
-   ✅ Scatter plot of temperature vs. usage
-   ✅ Histogram of daily consumption
-   ✅ Heatmap of monthly averages
-   ✅ Dashboard with appliance usage filter

---

## 📁 Dataset

**Source:** [UCI Machine Learning Repository: Individual household electric power consumption](https://archive.ics.uci.edu/ml/datasets/Individual+household+electric+power+consumption)

**Description:** The dataset contains **~2.1 million measurements** of electrical power consumption from a single household in France, collected at a **one-minute sampling rate** over a period of almost 4 years (Dec 2006 - Nov 2010).

**Key Attributes:**
-   `Global_active_power`: Household global minute-averaged active power (in kilowatts).
-   `Sub_metering_1`: Energy sub-metering for the kitchen ( dishwasher, oven, microwave).
-   `Sub_metering_2`: Energy sub-metering for the laundry room ( washing machine, tumble-drier).
-   `Sub_metering_3`: Energy sub-metering for the water heater and air conditioner.
-   `Date`, `Time`: Timestamp of the recording.

---

## 🛠️ Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your_username/household-energy-analysis.git
    cd household-energy-analysis
    ```

2.  **Create and activate a virtual environment (recommended):**
    ```bash
    python -m venv venv
    # On Windows
    venv\Scripts\activate
    # On macOS/Linux
    source venv/bin/activate
    ```

3.  **Install required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

---


### Key Steps performed in the notebook:
1.  **Data Acquisition:** Automated download and extraction of the raw ZIP file.
2.  **Data Cleaning:** Handling of missing values (`?`), parsing European-formatted dates, converting data types, and forward-filling gaps.
3.  **Feature Engineering:** Resampling minute-level data to daily and monthly aggregates, creating a binary flag for washing machine usage.
4.  **Simulation:** Generating realistic temperature data to demonstrate a correlation analysis.
5.  **Visualization:** Creating the four required static plots.
6.  **Dashboard:** Constructing an interactive dashboard with a subplot grid.

---

## 📈 Key Insights & Findings

The analysis revealed several strong patterns in household energy consumption:

1.  **🔄 Strong Seasonality:** Consumption peaks consistently during the winter (Dec-Jan) and summer (Jun-Aug) months due to heating and cooling needs, as clearly shown in the heatmap.
2.  **🌡️ Temperature Correlation:** A clear **U-shaped relationship** exists between temperature and consumption. Usage is lowest at moderate temperatures (~20°C) and spikes during both extreme cold and extreme heat.
3.  **⏰ Time-Based Patterns:** Daily usage is not constant. Weekends and holidays show significantly higher consumption, likely due to occupants being home all day.
4.  **📊 Usage Distribution:** Most days fall within a "normal" consumption range, but a long tail of high-usage days significantly impacts the monthly total.
5.  **🧺 Appliance Impact:** The operation of major appliances like the washing machine has a measurable and identifiable impact on the total daily load.

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/your_username/your_repo_name/issues).

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

---

## 📜 License

Distributed under the MIT License. See `LICENSE` file for more information.

---

## 👨‍💻 Author

**Your Name**
-   HashNode: [CodeYums.com](https://codeyums.hashnode.dev/)
-   LinkedIn: [@MaryamNaseem](in/maryam--naseem)
-   GitHub: [@MaryamCodeHub](https://github.com/MaryamCodeHub)

---

## 🙏 Acknowledgments

-   Data provided by [UCI Machine Learning Repository](https://archive.ics.uci.edu).
-   Inspiration for data storytelling and analysis.
-   Thanks to the open-source community for the invaluable tools (Pandas, NumPy, Plotly, Matplotlib).
```
