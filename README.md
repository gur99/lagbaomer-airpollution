# Lag BaOmer PM2.5 Analysis 🇮🇱

A data-driven study evaluating the impact of bonfire restrictions on **PM2.5 air pollution levels** in Israel during **Lag BaOmer** (2021–2025).  
This project is aimed at environmental researchers, public health policymakers, and data science students interested in real-world applications of statistical learning.

By combining public air quality data with non-parametric statistical analysis, the study explores whether regulatory bans on bonfires—particularly the **2025 national ban**—led to measurable improvements in urban air quality.

---

## Features

- 📊 **Air Quality Analysis** using real-world PM2.5 data from 11 urban stations across Israel.
- 🔬 **Statistical Testing** with Wilcoxon signed-rank test, Friedman test, and Bootstrap resampling (10,000 iterations).
- 📉 **Year-by-Year Comparisons** of pollution levels from 2021 to 2025.
- 📎 Visualizations including boxplots, PM2.5 trends, and bootstrap distributions.
- 🧠 Reproducible code written in Python for academic and public policy use.

---

##  Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/lagbaomer-pm25.git
   cd lagbaomer-pm25
   ```

2. **Set up a virtual environment (optional but recommended)**
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Open the analysis notebook**
   ```bash
   jupyter notebook notebooks/PM25_Analysis.ipynb
   ```

---

## Usage

You can reproduce the full analysis by running the Jupyter notebook:

```python
# Load the PM2.5 dataset
import pandas as pd
df = pd.read_csv('data/pm25_lagbaomer_2021_2025.csv')

# Perform Wilcoxon test comparing 2025 to 2021
from scipy.stats import wilcoxon
stat, p = wilcoxon(df['pm2021'], df['pm2025'])
print(f'p-value: {p}')
```


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
lagbaomer-pm25/
│
├── data/                      # Raw and cleaned data files
│   └── pm25_lagbaomer_2025.csv
│
├── notebooks/                 # Jupyter notebooks
│   └── PM25_Analysis.ipynb
│
├── README.md
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

## 📬 Contact & Acknowledgments

**Author:** Gur Yitzhaki  
**Affiliation:** Ruppin Academic Center – Statistical Learning (Final Project)  
**Email:** [gur.yitzhaki@gmail.com]  
**Data Source:** [Ministry of Environmental Protection – Air Quality Portal](https://www.sviva.gov.il)

Special thanks to the instructors of the Statistical Learning course and peers who provided feedback throughout this project.
---
