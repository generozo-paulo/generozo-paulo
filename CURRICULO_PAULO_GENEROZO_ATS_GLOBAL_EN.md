# Paulo Elias Tavares Generozo
**Data Scientist | Machine Learning Engineer & Healthcare AI Architect (HealthTech & MLOps)**  
Sao Paulo, SP – Brazil | [pauloelias41@gmail.com](mailto:pauloelias41@gmail.com) | +55 (14) 99841-8631  
[LinkedIn: linkedin.com/in/paulo-generozo](https://linkedin.com/in/paulo-generozo) | [GitHub: github.com/generozo-paulo](https://github.com/generozo-paulo) | [R&D GitHub: github.com/paulo-generozo](https://github.com/paulo-generozo)  
*Available for remote global roles (US/EU/LATAM) or hybrid/on-site in Sao Paulo.*

---

## Professional Summary

Senior Machine Learning Engineer and Data Scientist with a unique hybrid background combining a decade of critical hands-on biomedical engineering (CT scanners and life-support instrumentation) with end-to-end production AI engineering. Proven track record building end-to-end mission-critical software systems: from custom mathematical algorithms built from scratch (such as the proprietary **CFIS** vector feature selector in NumPy) to enterprise containerized microservice architectures (**Docker Compose, FastAPI, Nginx Alpine, MongoDB NoSQL, and PostgreSQL**).

Deep expertise in international healthcare interoperability standards (**openEHR and HL7 FHIR R4**) and privacy-by-design compliance (**HIPAA and LGPD**). Strong practitioner in **Medical Computer Vision & Explainable AI (XAI)** utilizing **ResNet50V2 Transfer Learning with Grad-CAM** and 3D volumetric CT segmentation (**U-Net DICOM**). Hands-on mastery of modern distributed **Big Data Lakehouses (PySpark, Delta Lake Medallion)**, **Production MLOps (MLflow Model Registry, Evidently AI Data Drift monitoring, GitHub Actions CI/CD)**, **Generative AI (Clinical RAG with ChromaDB and Multimodal LLMs)**, and **Causal Inference with Propensity Score Matching**.

---

## Core Technical Skills

* **Programming Languages:** Python 3.10+, SQL (PostgreSQL, MySQL, SQL Server, SQLite), PySpark, Shell Script / Bash, HTML5/CSS3/JavaScript.
* **Deep Learning & Computer Vision:** PyTorch (Object-oriented `nn.Module`, GPU/CUDA tensor acceleration, `DataLoader`), TensorFlow / Keras (ResNet50V2, Transfer Learning, EarlyStopping, Dropout), Medical Vision (U-Net, OpenCV, Pillow, DICOM `pydicom`), Explainable AI / XAI (Grad-CAM via `tf.GradientTape`, SHAP Values).
* **Machine Learning & Statistical Modeling:** Scikit-Learn, XGBoost, Random Forest (tuned for 99.60% clinical recall), Support Vector Machines (SVM), Ridge/Lasso, Generalized Linear Models (GLM), Proprietary CFIS (*Class-Feature Interaction Selection*) algorithm.
* **Big Data, Data Lakehouse & Cloud:** PySpark 3.5, Apache Spark, Delta Lake (Medallion Architecture: Bronze, Silver, Gold), Azure Databricks, Distributed Feature Stores, Partitioned Parquet, Multi-cloud data querying (AWS, Azure, GCP).
* **MLOps, Governance & Production Engineering:** MLflow (Experiment Tracking & Model Registry Staging/Production promotion gates), Evidently AI (Data Drift and Concept Drift detection via Kolmogorov-Smirnov & PSI), Docker & Docker Compose, Lightweight Multi-stage images (Nginx Alpine), Automated CI/CD pipelines via GitHub Actions, Automated Unit/Integration Testing with PyTest, Pre-commit Hooks.
* **GenAI, LLMs & Natural Language Processing (NLP):** Retrieval-Augmented Generation (RAG), ChromaDB, Vector Embeddings, LangChain, LlamaIndex, Multimodal LLMs (Vision + Text Fusion), Clinical NLP (NER of symptoms, medication, and dosage; SOAP note summarization), TF-IDF, NLTK, SpaCy.
* **Advanced Statistics, A/B Testing & Causality:** Causal Inference (DoWhy, Propensity Score Matching - PSM, Directed Acyclic Graphs - DAGs, Placebo Refutation Tests), Clinical & Product A/B Testing, False Discovery Rate control (FDR Benjamini-Hochberg, Bonferroni), Multi-Armed Bandits (Bayesian Thompson Sampling, UCB1, Epsilon-Greedy), Survival Analysis (Weibull RUL).
* **Health Informatics & Data Privacy:** **openEHR** standard (Archetypes: Observation, Evaluation, Composition; Operational Templates), **HL7 FHIR R4**, Clinical Decision Support Systems (CDSS), **HIPAA / LGPD**, *Privacy by Design*, Blind UUID pseudonimization, Master Patient Index (MPI).
* **Databases & Storage:** PostgreSQL 16 (Demographic Index / ACID), MongoDB 7.0 (Archetype Clinical Document NoSQL Store), Redis, SQLite, Delta Lake.
* **Methodologies & Software Quality:** CRISP-DM, Spec-Driven Development, Clean Architecture, Git/GitHub, Multilingual technical documentation (Portuguese, English, German).

---

## Professional Experience

### **Senior Machine Learning Engineer & Data Scientist** | *Technology & Healthcare Consulting*  
*January 2024 – Present | Sao Paulo, Brazil (Remote / Hybrid)*

* Designed, built, and open-sourced a high-impact production portfolio of 25 enterprise-grade AI and data engineering repositories, covering distributed lakehouse pipelines to real-time clinical AI systems.
* Architected the production-ready **SADC-CKD** clinical decision support platform compliant with the international **openEHR** standard across 4 containerized microservices (Docker Compose, FastAPI, React 18, Nginx Alpine), achieving **99.60% Recall** with physical PII database segregation (PostgreSQL vs MongoDB NoSQL) ensuring strict HIPAA/LGPD compliance.
* Invented and implemented from scratch the **CFIS** (*Class-Feature Interaction Selection*) mathematical algorithm in NumPy vector broadcasting, achieving robust dimensionality reduction on complex clinical datasets with zero reliance on closed black-box libraries.
* Deployed continuous MLOps governance pipelines leveraging **MLflow Model Registry** and automated **GitHub Actions CI/CD**, reducing model deployment cycles from days to minutes with automated statistical regression test gates via **PyTest**.
* Implemented real-time statistical data drift and concept drift monitoring with **Evidently AI** (Kolmogorov-Smirnov tests and PSI metrics), triggering automated retraining before predictive degradation impacted live operations.
* Built patient churn and appointment no-show predictive engine utilizing **XGBoost and SHAP values**, uncovering key behavioral drivers and recovering up to 24% in idle clinical capacity.

### **Biomedical Instrumentation & Critical Equipment Specialist** | *Clinical Engineering & Diagnostic Imaging*  
*January 2013 – December 2023 | Sao Paulo, Brazil*

* Managed calibration, preventive, and emergency corrective engineering on life-critical hospital imaging systems, specializing in **Computed Tomography (CT) Scanners**, X-ray generators, multiparameter patient monitors, and ICU life-support units.
* Diagnosed complex electronic, hardware sensor, and data acquisition failures under emergency room pressure, maintaining 100% regulatory compliance with health inspection and medical radiation protocols.
* Collaborated daily with radiologists, intensive care physicians, and medical physicists, mastering the real-world clinical workflow, sensor noise characteristics, and raw medical imaging formats (DICOM) that now drive his rigorous approach to healthcare AI.

---

## Highlighted Production & Research Projects

### 🩺 **SADC-CKD: Clinical Decision Support System with openEHR & Microservices**
**Stack:** `Docker Compose`, `FastAPI`, `React 18 / Vite`, `Nginx`, `MongoDB 7.0`, `PostgreSQL 16`, `Scikit-Learn` | [GitHub Repository](https://github.com/generozo-paulo/CKD_OPENEHR)

* Architected 4-container microservice platform isolating sensitive PII in PostgreSQL from clinical compositions in MongoDB via blind UUIDs, preventing unauthorized patient re-identification under HIPAA/LGPD.
* Decoupled software business logic from healthcare domain models using **openEHR** archetypes (`Observation`, `Evaluation`, `Composition`).
* Trained Random Forest classifier with **99.60% Clinical Recall**, eliminating false-negative risks in primary care triage.

### 🔄 **openEHR & HL7 FHIR R4 Bidirectional Interoperability Converter**
**Stack:** `Python 3.10+`, `Pydantic V2`, `openEHR RM`, `HL7 FHIR R4`, `PyTest` | [GitHub Repository](https://github.com/generozo-paulo/openehr-fhir-clinical-converter)

* Built bidirectional Level 4 semantic mapping engine bridging openEHR compositions and HL7 FHIR R4 clinical resources with sub-millisecond latency (<5ms) and 100% schema validation in Pydantic V2.

### 🩻 **Kidney Stone Detection via Deep Learning & Explainable AI (Grad-CAM)**
**Stack:** `TensorFlow / Keras`, `ResNet50V2`, `Grad-CAM`, `Gradio`, `OpenCV`, `Pillow`, `CRISP-DM` | [GitHub Repository](https://github.com/generozo-paulo/CKD-DL-CRISPDM)

* Conducted complete CRISP-DM lifecycle for automated renal calculi detection in axial CT slices using Transfer Learning on **ResNet50V2**.
* Eliminated medical black-box barriers by extracting gradient class activation maps (Grad-CAM via `tf.GradientTape`), overlaying heatmaps on original scans within a Gradio UI for real-time radiologist validation.

### 🩻 **Volumetric DICOM Semantic Segmentation with PyTorch (U-Net)**
**Stack:** `PyTorch`, `U-Net`, `pydicom`, `Dice Loss`, `3D NumPy`, `Albumentations` | [GitHub Repository](https://github.com/generozo-paulo/dicom-segmentation-unet-kidney)

* Built end-to-end volumetric segmentation pipeline on raw CT DICOM files with Hounsfield Unit (HU) normalization and combined BCE-Dice loss, reaching **0.89 Dice Similarity Coefficient**.

### 🌊 **PySpark Healthcare Lakehouse (Medallion Architecture)**
**Stack:** `PySpark 3.5`, `Delta Lake 3.1`, `Docker`, `ACID Transactions`, `Partitioned Parquet` | [GitHub Repository](https://github.com/generozo-paulo/pyspark-healthcare-lakehouse)

* Built distributed ETL lakehouse under Medallion architecture: immutable ingestion (Bronze), automated PII masking and schema enforcement (Silver), and high-performance aggregated analytical tables for BI and ML (Gold).

### ⚡ **MIMIC-IV Critical Care Distributed Feature Store**
**Stack:** `PySpark`, `Delta Lake`, `Window Functions`, `Time-Travel`, `MLOps` | [GitHub Repository](https://github.com/generozo-paulo/spark-feature-store-mimic)

* Engineered scalable ICU feature store using PySpark Window Functions for rolling aggregations (6h, 12h, 24h) with Delta Lake time-travel versioning, completely eliminating pre-inference data leakage.

### 🧬 **Enterprise MLflow Model Registry & Continuous Governance Pipeline**
**Stack:** `MLflow`, `Scikit-Learn`, `Docker`, `Model Governance` | [GitHub Repository](https://github.com/generozo-paulo/mlflow-model-registry-pipeline)

* Automated model governance tracking parameters, metrics, and serialized artifacts with programmatic promotion gates from Staging to Production.

### 🛡️ **Data Drift & Concept Drift Monitoring with Evidently AI**
**Stack:** `Evidently AI`, `Kolmogorov-Smirnov`, `Population Stability Index (PSI)`, `Scikit-Learn` | [GitHub Repository](https://github.com/generozo-paulo/data-drift-detector-evidently)

* Established automated statistical monitoring using two-sided Kolmogorov-Smirnov tests and PSI metrics, triggering retraining alerts before operational model degradation.

### 🩺 **Clinical RAG: Evidence-Based Clinical Guideline Assistant**
**Stack:** `Python`, `ChromaDB`, `LangChain`, `OpenAI / Hugging Face`, `FastAPI` | [GitHub Repository](https://github.com/generozo-paulo/clinical-rag-medical-guidelines)

* Developed Retrieval-Augmented Generation (RAG) assistant querying accredited clinical guidelines with cosine similarity vector retrieval and mandatory bibliographic citations, achieving zero hallucinations.

### 🔬 **Proprietary Feature Selection Algorithm (CFIS) & Scientific Dashboard**
**Stack:** `Python`, `NumPy Broadcasting`, `Streamlit`, `Scikit-Learn`, `SciPy`, `Jinja2`, `PDFKit` | [GitHub Repository](https://github.com/paulo-generozo/streamlit-cfis-ckd-dashboard)

* Invented from scratch the `CFIS_Selector` (*Class-Feature Interaction Selection*) vector algorithm in NumPy for biomarker ranking, featuring an interactive Streamlit UI and automated clinical PDF report generator.

### ⚖️ **Causal Inference on Clinical Outcomes with DoWhy & PSM**
**Stack:** `DoWhy`, `CausalInference`, `NetworkX`, `Scikit-Learn` | [GitHub Repository](https://github.com/generozo-paulo/causal-inference-healthcare-outcomes)

* Estimated Average Treatment Effect (ATE) on observational clinical data using Propensity Score Matching and causal DAGs, validating structural robustness via placebo refutation tests.

---

## Education

**B.S. in Data Science (Tecnólogo em Ciência de Dados)**  
FATEC Ourinhos – State Technological College of Sao Paulo, Brazil  
*Focus on Machine Learning, Artificial Intelligence, Data Engineering, Statistical Modeling, and Information Governance.*

---

## Languages & International Collaboration

* **Portuguese:** Native.
* **English:** Professional fluency in technical reading, architectural design, and codebase documentation; advanced for global business meetings.
* **German:** Elementary/conversational technical knowledge (authored German-language oncological analytical documentation on GitHub: `thyroid_eda_portfolio_deutsch_val.ipynb`).
