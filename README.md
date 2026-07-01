# Carbon-Aware Scheduling of Data Centre Workloads

A machine learning project that forecasts UK grid carbon intensity and uses those forecasts to schedule data centre workloads into lower-carbon time windows.

## Project Overview
- Collected and preprocessed 17,500+ hourly UK grid carbon intensity readings via the Carbon Intensity API
- Engineered 24 lag features and trained Ridge regression and Random Forest models (MAE: 10.59 gCO₂/kWh)
- Built a linear programming scheduler using PuLP to shift flexible workloads to lower-carbon hours
- Achieved 4.49% carbon reduction, saving ~554,000 gCO₂ without dropping any workload

## Files
- `notebooks/01_api_dataset.ipynb` - Data collection, preprocessing, and forecasting models
- `notebooks/02_scheduler_pulp.ipynb` - Carbon-aware workload scheduler

## Technologies
Python, Pandas, NumPy, scikit-learn, PuLP, Matplotlib
