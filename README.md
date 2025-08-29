# Fuel Efficiency & Emissions — Data Storytelling Project

A clean, story-first analysis of 2014 vehicle fuel consumption and CO₂ emissions, with reproducible Python notebooks and a presentation for non-technical stakeholders.

## 🚀 What’s Inside
- **Notebook:** `fuel.ipynb` – data cleaning, EDA, key insights, and a simple predictive example.
- **Slides:** `Fuel_Efficiency_Fluency_Enhanced.pptx` – stakeholder-ready deck with limitations, roadmap, and ownership.
- **Report Notes:** Aligns with data fluency best practices (purpose, context, one-chart-one-insight, ownership, roadmap).

## 🧠 Key Questions We Answer
- How do engine size and cylinders affect CO₂ emissions?
- Which vehicle classes and fuel types are most/least efficient?
- City vs. highway fuel consumption — how big is the gap?
- What simple model can predict CO₂ using basic features?

## 📊 Highlights
- Larger engines/cylinders → higher CO₂.
- SUVs/Pickups consume the most; compacts perform best.
- City driving uses ~30% more fuel than highway.
- Manual vs automatic differences are small; model/tech matters.

## 🗂️ Project Structure
```
.
├── fuel.ipynb
├── Fuel_Efficiency_Fluency_Enhanced.pptx
├── data/
│   ├── raw/              # (optional) put raw datasets here
│   └── processed/        # (optional) cleaned/derived datasets
├── src/                  # (optional) reusable Python scripts
│   └── utils.py
└── README.md
```

## 🔧 Setup
1) **Create/activate environment (example using `venv`):**
```bash
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS/Linux
source .venv/bin/activate
```

2) **Install packages:**
```bash
pip install -U pandas numpy matplotlib scikit-learn jupyter python-pptx
# Optional (Power BI integration inside notebooks)
pip install powerbiclient
```

3) **Open Jupyter:**
```bash
jupyter notebook
```

## ▶️ Reproduce the Analysis
- Open `fuel.ipynb` and run cells top-to-bottom.
- If you store data locally, point the notebook to `data/raw/FuelConsumption.csv` (2014, 1067 rows).

## 🔗 Power BI Integration (Optional)
- Use Python for prep (feature engineering, modeling), export to `data/processed/*.parquet` or `.csv`.
- In Power BI, **Get Data → Folder/File** and build visuals.
- You can also add a **Python visual** to reuse matplotlib/plotly charts from the notebook.

## 📁 Data Source
- Government of Canada — Vehicle Fuel Consumption Ratings (2014) — `FuelConsumption.csv`

## 🗺️ Roadmap
- Add a small regression (regularized) + feature importance.
- Publish an interactive dashboard (Power BI).
- Consider an API/automated refresh for near–real-time updates.

## 📜 License
Choose a license (e.g., MIT). Update this section accordingly.
