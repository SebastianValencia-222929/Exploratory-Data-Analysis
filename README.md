# Exploratory Data Analysis

A collection of exploratory data analysis (EDA) projects using Python and Jupyter Notebooks. Each analysis covers a distinct dataset and set of research questions.

---

## Projects

### 1. SNI Exploratory Analysis — Phase 1
**Folder:** `SNI exploratory analysis/`

Analysis of Mexico's National Researchers System (SNI) historical data from [SECIHTI](https://secihti.mx/sistema-nacional-de-investigadores/archivo-historico/). It explores growth trends, knowledge area distributions, researcher levels, and territorial distribution, with a focused comparison between UACJ and UACH institutions in Chihuahua.

---

### 2. ENIF Exploratory Analysis — Phase 2
**Folder:** `ENIF exploratory analysis/`

Analysis of the ENIF 2024 microdata from INEGI to study financial access in Mexico. Topics include payroll and personal credit demographics, financial inclusion gaps between indigenous and non-indigenous populations, cryptocurrency adoption patterns, and fraud profiles.

**Additional dependency:** `ftfy` and `pyarrow` (installed inside the notebook with `pip install ftfy pyarrow`).

---

### 3. Transfer Market Analysis Summer 2025
**Folder:** `Transfer Market Analysis Summer 2025/`

Exploratory analysis of the summer 2025 football transfer window dataset from Kaggle.  
Dataset source: [Kaggle — 2025 Summer Football Transfer Window](https://www.kaggle.com/datasets/abdellahmaghous/2025-summer-football-transfer-window)

It examines player movements, market values, transfer fees, loan vs. permanent deals, and league/country trends.

---

## Requirements

- Python 3.8+
- Jupyter Notebook or Google Colab (notebooks were originally built for Colab)

Install the core Python dependencies:

```bash
pip install numpy pandas matplotlib plotly seaborn ftfy pyarrow
```

---

## How to Run

### Option A — Google Colab (recommended)

1. Open [Google Colab](https://colab.research.google.com/).
2. Upload the desired `.ipynb` file or open it directly from GitHub.
3. Follow the in-notebook instructions to mount Google Drive or upload the dataset file when prompted.
4. Run all cells (`Runtime > Run all`).

### Option B — Local Jupyter Notebook

1. Clone the repository:
   ```bash
   git clone https://github.com/SebastianValencia-222929/Exploratory-Data-Analysis.git
   cd Exploratory-Data-Analysis
   ```

2. Install dependencies:
   ```bash
   pip install numpy pandas matplotlib plotly seaborn ftfy pyarrow notebook
   ```

3. Launch Jupyter:
   ```bash
   jupyter notebook
   ```

4. Open the desired `.ipynb` file from the Jupyter file browser.

5. **Important:** Notebooks that use `google.colab` (drive mount or file upload) must have those cells replaced with local file paths before running locally. For example, replace:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```
   with the local path to the dataset file:
   ```python
   df = pd.read_csv('path/to/your/dataset.csv')
   ```

---

## Dataset Sources

| Project | Source |
|---------|--------|
| SNI | [SECIHTI — Archivo Histórico SNI](https://secihti.mx/sistema-nacional-de-investigadores/archivo-historico/) |
| ENIF | [INEGI — ENIF 2024](https://www.inegi.org.mx/programas/enif/2024/) |
| Transfer Market | [Kaggle — 2025 Summer Football Transfer Window](https://www.kaggle.com/datasets/abdellahmaghous/2025-summer-football-transfer-window) |
