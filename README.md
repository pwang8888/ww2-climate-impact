# 🌍 Temperature Data Mining: WWII Case Study (Germany & Japan)

> **Portfolio Edition** 
> A data analytics and causal inference study on whether **World War II human activities** (e.g., urban destruction, industrial shifts) left **measurable signals** in historical **Earth surface temperature** records.

---

## 📌 Highlights
- **Time-series modeling:** Auto-ARIMA for trend/seasonality  
- **Causal inference:** Synthetic Control Method (SCM) to build counterfactuals  
- **Cross-language workflow:** Python ↔️ R via `rpy2` inside Jupyter  
- **Reproducibility:** SQLite-backed data prep + notebooks  

---

## 📂 Data
- `GlobalTemperatures.csv` — global monthly averages (~1750–2013)  
- `GlobalLandTemperaturesByCountry.csv` — country-level monthly averages (~1700–2013)  

> Place raw data under `data/` (not included here). Update notebook paths as needed.

---

## ⚙️ Setup
```bash
# 1) Create environment (Python 3.10+ recommended)
python -m venv .venv && source .venv/bin/activate  # macOS/Linux
# or: python -m venv .venv; .venv\Scripts\activate  # Windows

# 2) Install dependencies
pip install -r requirements.txt

# 3) (Optional) Jupyter kernel
python -m ipykernel install --user --name ww2-climate

