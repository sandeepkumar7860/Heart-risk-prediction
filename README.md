# Heart-risk-prediction
# ML Predictor (Django)

Simple Django site that loads your uploaded pickled artifacts (`knn_heart_model.pkl`, `heart_scaler.pkl`, `heart_columns.pkl`) from the project root and provides a form to submit comma-separated features for prediction.

Setup (Windows):

1. Create and activate a virtual environment:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

2. Install dependencies:

```powershell
pip install -r requirements.txt
```

3. Run migrations and start server:

```powershell
python manage.py migrate
python manage.py runserver
```

4. Open http://127.0.0.1:8000/ and enter comma-separated features to predict.

Notes:
- The project expects the three pickle files to be placed in the project root (same folder as `manage.py`).
- Enter feature values in the same order as the `heart_columns.pkl` list if available.
