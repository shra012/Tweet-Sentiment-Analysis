# Notebook-only Pipeline (Prep, Models, Search)
All components are notebooks. Run them in order:

- `00_shared_utils.ipynb` — shared cleaning + feature builders (import with `%run`)
- `01_eda.ipynb` — dataset exploration & artifacts
- `02_prep_preview.ipynb` — shows cleaned features preview
- `03_baselines.ipynb` — Logistic Regression & Multinomial NB + calibration (saves best pipeline)
- `04_trees_xgb_shap.ipynb` — RandomForest/XGBoost + SHAP
- `05_semantic_search.ipynb` — embeddings + FAISS index (optional)
- `06_infer.ipynb` — batch scoring with a saved pipeline

Artifacts land in `artifacts/` and models in `model_registry/`.
If a package is missing, use the commented `%pip install ...` line in each notebook when running locally.
