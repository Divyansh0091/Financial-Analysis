# Financial_Data_Analysis_&_Cleaning Pipeline

A complete Python data analytics project that transforms raw, messy corporate financial transactional logs into clean, structured, and visually auditable business intelligence assets.

---

## 📊 Project Visual Overview
Here is the final comparison visualization engineered from the melted long-form financial dataset:

![Financial Chart](Chart.png)

---

## 🧠 Core Engineering Phases & Logic Covered

### 1. Advanced Data Imputation & Diagnostics
- **Handling Missing Values:** Identified and resolved missing data within critical metrics using statistical imputation (median-based grouping).
- **Data Standardization:** Converted mixed-cased text anomalies (e.g., 'success', 'SUCCESS', 'failed') into a uniform corporate standard.

### 2. Outlier Identification & Remediation
- **Anomaly Detection:** Detected calculation errors and rogue data markers (like `9999.0` and `-500.0` values).
- **In-place Correction:** Used advanced logical index mapping via `.loc` constraints to replace toxic outliers with clean median baselines.

### 3. Data Transformation & Reshaping (Wide-to-Long)
- **The Challenge:** The source schema stored business metrics horizontally (`Revenue_Lakhs` and `Expenses_Lakhs` side-by-side).
- **The Melt Execution:** Leveraged `pd.melt()` to compress multi-column metrics into indexed rows, mapping transactional profiles into a centralized categorical matrix (`Financial_Metric` and `Amount`).

---

## 🛠️ Tech Stack & Technical Competencies Tested
- **Language:** Python 3.x
- **Core Engineering:** Pandas (DataFrames, Loc manipulation, Melt reshaping), NumPy
- **Data Visualization:** Seaborn, Matplotlib Pyplot
- **Environment:** Jupyter Notebook
- **Version Control:** Git / GitHub Desktop

