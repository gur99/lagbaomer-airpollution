# Lag BaOmer PM2.5 Analysis 

A data-driven study evaluating the impact of bonfire restrictions on **PM2.5 air pollution levels** in Israel during **Lag BaOmer** (2021–2025).  
This project is aimed at environmental researchers, public health policymakers, and data science students interested in real-world applications of statistical learning.

By combining public air quality data with non-parametric statistical analysis, the study explores whether regulatory bans on bonfires—particularly the **2025 national ban**—led to measurable improvements in urban air quality.

---

## Features

- **Air Quality Analysis** using real-world PM2.5 data from 11 urban stations across Israel.
- **Statistical Testing** with Wilcoxon signed-rank test, Friedman test, and Bootstrap resampling (10,000 iterations).
- **Year-by-Year Comparisons** of pollution levels from 2021 to 2025.
- Visualizations including boxplots, PM2.5 trends, and bootstrap distributions.
- Reproducible code written in Python for academic and public policy use.

---

##  Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/lagbaomer-pm25.git
   cd lagbaomer-pm25
   ```

2. **Open the analysis notebook**
   ```bash
   jupyter notebook notebooks/reaserch_python.ipynb
   ```
---


##  Technologies Used

- **Python 3.8+**
- `pandas` – data wrangling
- `numpy` – numerical operations
- `scipy` – statistical tests
- `matplotlib` / `seaborn` – data visualization
- `jupyter` – interactive analysis

---

##  Project Structure

```plaintext
Lagbaomer-airpollution Project/
│
├── Article/
│   └── LagBaOmer_AirPollution_Study_2025
│
├── data/
│   ├── Holiday_Eve/
│   │   ├── 2021_HolidayEve.xlsx
│   │   ├── 2022_HolidayEve.xlsx
│   │   ├── 2023_HolidayEve.xlsx
│   │   ├── 2024_HolidayEve.xlsx
│   │   └── 2025_HolidayEve.xlsx
│   │
│   └── WeeklyReports/
│       ├── WeeklyReport2021.xlsx
│       ├── WeeklyReport2022.xlsx
│       ├── WeeklyReport2023.xlsx
│       ├── WeeklyReport2024.xlsx
│       └── WeeklyReport2025.xlsx
│
├── notebooks/
│   └── reaserch_python.ipynb
│
├── visualizations/
│   └── PM25_Comparison_2021_vs_2025.html
│
└── README.md
```

---

##  Contributing

Contributions, issues, and suggestions are welcome!  
To contribute:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add YourFeature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a pull request

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

**Author:** Gur Yitzhaki  
**Data Source:** [Ministry of Environmental Protection – Air Quality Portal](https://www.sviva.gov.il)


Special thanks to the instructors of the Statistical Learning course and peers who provided feedback throughout this project.
