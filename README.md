# Hi, I'm Alexander Amiri

Data Scientist with 2+ years of experience building end-to-end ML systems — from data pipelines to production — including LLM pipelines for clinical data at UCSF, a live MLOps platform serving daily predictions, and fraud detection across 6.3M+ transactions.

Currently a Data Scientist at Hedwig Xpress, and previously built clinical NLP/LLM pipelines at UCSF Radiation Oncology. M.S. in Data Science and Artificial Intelligence from the University of San Francisco, B.S. in Statistical Data Science from UC Davis.

Open to Data Science / ML Engineering roles.

## Projects

### [Hikeability](https://hike-ability.com) — Trail Conditions Platform ([repo](https://github.com/cyab05/hikeability))

An end-to-end MLOps pipeline classifying **3,500+ Washington hiking trails** daily as hikeable/modest/unhikeable, prompting NVIDIA Nemotron 49B with trip reports, weather forecasts, and closure alerts — **98% accuracy** on a human-validated evaluation set.

- Nightly data pipeline via GitHub Actions and Docker, scraping WTA trip reports and Open-Meteo weather data, running LLM inference on a GCP VM, and serving predictions to a live Mapbox web app with zero manual intervention
- Evaluated 6 model configurations (2 model sizes × 3 prompting strategies) tracked in MLflow, selecting one-shot prompting as the optimal strategy balancing 100% accuracy and minimal token cost over few-shot alternatives

`Python` `NVIDIA Nemotron 49B` `GitHub Actions` `Docker` `GCP` `Mapbox GL JS` `MLflow`

### Fraud Detection Pipeline

A fraud detection pipeline ingesting **6.3M+ transactions** with 8 engineered features, addressing a 0.13% fraud-rate class imbalance via undersampling.

- Trained 4 PySpark classifiers (GBT, RF, DT, LR); GBT achieved **0.9994 ROC-AUC** and **0.9998 F1** on a 1.27M-row test set
- Random Forest importance isolated 8 top predictive features

`Python` `PySpark` `Apache Airflow` `MongoDB` `GCP Dataproc` `GCS`

### Clinical LLM Summarization & Matching — UCSF Radiation Oncology

Supporting cancer survival prediction research, this pipeline compresses 100K+ token clinical notes to 500 tokens (80% reduction) via an LLM summarization pipeline (Qwen2.5/Ollama), enabling BioClinicalBERT ingestion across 7 glioma follow-up timepoints. Processed 64K MRI studies and 26K pathology reports across 12K patients to produce 50K MRI–pathology training pairs. Fine-tuned encoder LLMs via LoRA and contrastive learning (MNRL), improving matched-pair cosine similarity from 0.63 to 0.79 across 70K patient-timepoint pairs. *(Clinical work, code private.)*

`Python` `LoRA` `Contrastive Learning` `BioClinicalBERT` `Ollama`

## Tech

**Programming** — Python, SQL, NoSQL, R

**ML & Statistics** — Regression, Classification, Decision Trees, Random Forest, XGBoost, Deep Learning, NLP, LLMs, LLM Fine-Tuning (LoRA), Contrastive Learning, Embedding Models, Prompt Engineering, Statistical Modeling, A/B Testing, Causal Inference, ETL and Data Pipelines, Data Visualization

**Tools** — PyTorch, TensorFlow, Scikit-Learn, HuggingFace Transformers, vLLM, PySpark, Spark, Pandas, NumPy, Matplotlib, Seaborn, Plotly, Apache Airflow, GitHub Actions, MLflow, MongoDB, Ollama, Kubernetes, Terraform, Git/GitHub, Google Cloud (Vertex AI, Cloud Run, Dataproc, GCS), Docker, Tableau

## Connect

[LinkedIn](https://linkedin.com/in/alex-amiri) · [alexamiri4242@gmail.com](mailto:alexamiri4242@gmail.com)
