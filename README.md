<div align="center">

# 🩺 Paulo Elias Tavares Generozo
### **Senior Data Scientist | Machine Learning & Healthcare AI Architect**
#### *Bridging Critical Biomedical Engineering with Production-Grade MLOps & Distributed AI*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/paulo-generozo)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:pauloelias41@gmail.com)
[![GitHub P&D](https://img.shields.io/badge/GitHub_R%26D-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/paulo-generozo)
[![Resume](https://img.shields.io/badge/Curriculo_ATS-2563EB?style=for-the-badge&logo=read-the-docs&logoColor=white)](https://github.com/generozo-paulo/generozo-paulo/blob/main/CURRICULO_PAULO_GENEROZO_ATS_SENIOR.md)

São Paulo, Brazil 🇧🇷 | Available for **Remote Global Roles (US / EU / Worldwide)** & Hybrid/On-site in SP

---

</div>

## 🧭 Executive Summary & The Asymmetric Moat

I am a Senior Machine Learning Engineer and Data Scientist with an uncommon hybrid background: **a decade of hands-on mission-critical experience in hospital biomedical engineering** (calibrating Computed Tomography scanners and life-support units) combined with **production-grade AI and distributed software engineering**.

This gives me an irreplaceable edge in mission-critical environments: I understand the physical nature of sensor noise, raw DICOM radiography, and healthcare workflows from the hospital floor to the server rack.

### 🌟 Core Differentiators:
* 🩺 **HealthTech & Level 4 Interoperability:** Production implementation of the international **openEHR** standard (Archetypes & Compositions) and **HL7 FHIR R4**, architected under strict **Privacy by Design (LGPD/HIPAA)**.
* 🔬 **Math & Algorithms From Scratch:** Creator of the proprietary **CFIS** (*Class-Feature Interaction Selection*) vector algorithm in pure NumPy broadcasting.
* 🩻 **Computer Vision & Explainable AI (XAI):** ResNet50V2 Transfer Learning paired with **Grad-CAM** thermal maps (`tf.GradientTape`) and volumetric 3D CT segmentation with **PyTorch U-Net (0.89 Dice)**.
* 🌊 **Big Data & Distributed Lakehouses:** **PySpark 3.5 & Delta Lake** Medallion Lakehouses with ACID transactions, time-travel, and scalable feature stores on MIMIC-IV ICU data.
* ⚙️ **End-to-End MLOps & Governance:** **MLflow Model Registry** gates, continuous **Evidently AI** data/concept drift monitoring, Docker multi-stage builds, and automated **GitHub Actions CI/CD** with PyTest regression testing.
* ⚖️ **Statistical Rigor & Causal Inference:** Clinical A/B testing with False Discovery Rate (FDR) control and Causal Inference via **DoWhy & Propensity Score Matching (PSM)**.

---

## 🏛️ System Architecture Showcase: Enterprise HealthTech SADC

```
┌─────────────────────────────────────────────────────────────────────────────────────────┐
│                    SADC-CKD: CLINICAL DECISION SUPPORT MICROSERVICES                    │
│                                                                                         │
│   ┌─────────────────────┐       HTTP / JSON        ┌────────────────────────────────┐  │
│   │   sadc-frontend     │ ───────────────────────> │           sadc-api             │  │
│   │   (React 18 + Vite) │ <─────────────────────── │      (FastAPI Assíncrono)      │  │
│   │   Served by Nginx   │                          └──────────────┬─────────────────┘  │
│   └─────────────────────┘                                         │                     │
│                                                                   │                     │
│               ┌───────────────────────────────────────────────────┴─────────────┐       │
│               │                                                                 │       │
│               ▼                                                                 ▼       │
│   ┌────────────────────────┐                                  ┌─────────────────────┐   │
│   │  Master Patient Index  │                                  │   Clinical Store    │   │
│   │  PostgreSQL 16 Alpine  │                                  │     MongoDB 7.0     │   │
│   │  (PII / Identificável) │                                  │ (openEHR Archetypes)│   │
│   └────────────────────────┘                                  │ Linked only by UUID │   │
│                                                               └─────────────────────┘   │
│               ▲                                                                 ▲       │
│               └───────────── PRIVACY BY DESIGN (LGPD / HIPAA) ──────────────────┘       │
│                           Physical Database Segregation                                 │
└─────────────────────────────────────────────────────────────────────────────────────────┘
```

---

## 🚀 Highlighted Engineering Portfolio (25 Production Repositories)

### 1. 🩺 HealthTech, Medical AI & Interoperability
| Repository | Technology Stack | Key Metrics & Highlights |
| :--- | :--- | :--- |
| **[CKD_OPENEHR](https://github.com/generozo-paulo/CKD_OPENEHR)** | Docker Compose, FastAPI, React 18, Nginx, MongoDB, Postgres | **99.60% Recall**, openEHR Level 4 Compositions, LGPD PII segregation. |
| **[openehr-fhir-clinical-converter](https://github.com/generozo-paulo/openehr-fhir-clinical-converter)** | Python 3.10+, Pydantic V2, openEHR RM, HL7 FHIR R4 | Bidirectional translation engine with **<5ms latency** per clinical transaction. |
| **[CKD-DL-CRISPDM](https://github.com/generozo-paulo/CKD-DL-CRISPDM)** | TensorFlow/Keras, ResNet50V2, Grad-CAM, Gradio, OpenCV | Explainable AI via **Grad-CAM** thermal maps eliminating medical black-box barriers. |
| **[dicom-segmentation-unet-kidney](https://github.com/generozo-paulo/dicom-segmentation-unet-kidney)** | PyTorch, U-Net, pydicom, Hounsfield Units (HU) | Volumetric 3D CT segmentation reaching **0.89 Dice Similarity**. |
| **[biomedical-signal-anomaly-detector](https://github.com/generozo-paulo/biomedical-signal-anomaly-detector)** | SciPy DSP, Pan-Tompkins, PyTorch Autoencoders | **98.7% sensitivity** in detecting real-time cardiac arrhythmia in ECG telemetry. |

### 2. ⚙️ MLOps, CI/CD & Model Governance
| Repository | Technology Stack | Key Metrics & Highlights |
| :--- | :--- | :--- |
| **[mlflow-model-registry-pipeline](https://github.com/generozo-paulo/mlflow-model-registry-pipeline)** | MLflow, Scikit-Learn, Docker, Model Governance | Automated staging-to-production promotion gates with complete artifact lineage. |
| **[data-drift-detector-evidently](https://github.com/generozo-paulo/data-drift-detector-evidently)** | Evidently AI, Kolmogorov-Smirnov, PSI, Scikit-Learn | Continuous statistical drift monitoring triggering proactive retraining alerts. |
| **[automated-ci-cd-model-deploy](https://github.com/generozo-paulo/automated-ci-cd-model-deploy)** | GitHub Actions, Docker multi-stage, FastAPI, PyTest | Zero-downtime automated deployment with automated regression test gates. |
| **[iris-classification-en](https://github.com/generozo-paulo/iris-classification-en)** | Python 3.12, Docker Compose, XGBoost, PyTest | Production-ready CRISP-DM pipeline with 100% automated test coverage. |

### 3. 🌊 Big Data, Lakehouse & Distributed Feature Stores
| Repository | Technology Stack | Key Metrics & Highlights |
| :--- | :--- | :--- |
| **[pyspark-healthcare-lakehouse](https://github.com/generozo-paulo/pyspark-healthcare-lakehouse)** | PySpark 3.5, Delta Lake 3.1, ACID, Partitioned Parquet | Medallion architecture (Bronze/Silver/Gold) with automated PII masking. |
| **[spark-feature-store-mimic](https://github.com/generozo-paulo/spark-feature-store-mimic)** | PySpark, Delta Lake, Window Functions, Time-Travel | Distributed ICU feature store preventing 100% of pre-inference data leakage. |
| **[azure-databricks-churn-etl](https://github.com/generozo-paulo/azure-databricks-churn-etl)** | Azure Databricks, PySpark, Delta Lake, Cloud ETL | Scalable telemetry pipeline optimizing cloud costs through smart partitioning. |

### 4. 🧠 Generative AI, LLMs & Multimodal Systems
| Repository | Technology Stack | Key Metrics & Highlights |
| :--- | :--- | :--- |
| **[clinical-rag-medical-guidelines](https://github.com/generozo-paulo/clinical-rag-medical-guidelines)** | ChromaDB, LangChain, Embeddings, FastAPI | Clinical RAG with cosine similarity and **mandatory source citations** (zero hallucination). |
| **[medical-records-summarizer-llm](https://github.com/generozo-paulo/medical-records-summarizer-llm)** | Transformers, SpaCy Clinical, Pydantic, RegEx Sanitizer | Automated SOAP note summarization with 100% PII de-identification before inference. |
| **[multimodal-medical-report-generator](https://github.com/generozo-paulo/multimodal-medical-report-generator)** | PyTorch, Vision Transformers (ViT), Multimodal LLM | Multimodal feature fusion aligning medical radiography scans with clinical histories. |

### 5. 📈 Statistical Experimentation, Causal Inference & Business ROI
| Repository | Technology Stack | Key Metrics & Highlights |
| :--- | :--- | :--- |
| **[clinical-ab-testing-framework](https://github.com/generozo-paulo/clinical-ab-testing-framework)** | Statsmodels, SciPy, FDR Benjamini-Hochberg | Statistical power sizing (MDE), non-parametric hypothesis tests, and multiple testing correction. |
| **[causal-inference-healthcare-outcomes](https://github.com/generozo-paulo/causal-inference-healthcare-outcomes)** | DoWhy, Propensity Score Matching (PSM), DAGs | Average Treatment Effect (ATE) estimation validated via placebo refutation tests. |
| **[multi-armed-bandit-triage](https://github.com/generozo-paulo/multi-armed-bandit-triage)** | NumPy, Thompson Sampling, UCB1, Epsilon-Greedy | **42% cumulative regret reduction** compared to static traditional A/B testing. |
| **[equipment-predictive-maintenance-roi](https://github.com/generozo-paulo/equipment-predictive-maintenance-roi)** | Lifelines, Weibull Survival Analysis, Monte Carlo | Remaining Useful Life (RUL) modeling showing **up to 38% reduction** in downtime costs. |
| **[patient-churn-and-no-show-analyzer](https://github.com/generozo-paulo/patient-churn-and-no-show-analyzer)** | XGBoost, SHAP Values, CRISP-DM, FastAPI | **0.88 AUC-ROC** identifying key behavioral churn drivers and recovering idle revenue. |

### 6. 🔬 Core Math, R&D & Algorithms From Scratch
| Repository | Technology Stack | Key Metrics & Highlights |
| :--- | :--- | :--- |
| **[streamlit-cfis-ckd-dashboard](https://github.com/paulo-generozo/streamlit-cfis-ckd-dashboard)** | NumPy Broadcasting, Streamlit, SciPy, Jinja2 | Proprietary CFIS algorithm benchmarking univariant ANOVA vs Gini importance. |
| **[DEEP_LEARNING_TITANIC](https://github.com/paulo-generozo/DEEP_LEARNING_TITANIC)** | PyTorch (`nn.Module`), GPU/CUDA, `DataLoader` | Object-oriented deep neural network with custom mini-batches and Dropout regularizers. |
| **[PLN-FERNANDO-PESSOA](https://github.com/paulo-generozo/PLN-FERNANDO-PESSOA)** | Keras/TensorFlow, TF-IDF, NLTK, BeautifulSoup4 | **80.0% accuracy** on 4 literary heteronyms with confidence threshold rejection. |
| **[Thyroid-Cancer](https://github.com/generozo-paulo/Thyroid-Cancer)** | Jupyter, Pandas, Scikit-Learn, CRISP-DM | Bilingual clinical predictive modeling and EDA published in **Portuguese & German**. |

---

## 🛠️ Comprehensive Tech Stack

<div align="center">

| Domain | Technologies |
| :--- | :--- |
| **Languages** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-025E8C?style=flat-square&logo=database&logoColor=white) ![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apache-spark&logoColor=white) ![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnu-bash&logoColor=white) |
| **Deep Learning & Vision** | ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white) ![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white) ![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white) ![Keras](https://img.shields.io/badge/Keras-D00000?style=flat-square&logo=keras&logoColor=white) |
| **Machine Learning & Stats** | ![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white) ![XGBoost](https://img.shields.io/badge/XGBoost-EB2E2E?style=flat-square) ![Statsmodels](https://img.shields.io/badge/Statsmodels-00599C?style=flat-square) |
| **Big Data & Lakehouse** | ![Apache Spark](https://img.shields.io/badge/Apache_Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white) ![Delta Lake](https://img.shields.io/badge/Delta_Lake-00A4E4?style=flat-square) ![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white) |
| **MLOps & DevOps** | ![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white) ![PyTest](https://img.shields.io/badge/PyTest-0A9EDC?style=flat-square&logo=pytest&logoColor=white) |
| **Databases** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white) |
| **Healthcare Standards** | ![openEHR](https://img.shields.io/badge/openEHR-Level_4_RM-brightgreen?style=flat-square) ![HL7 FHIR](https://img.shields.io/badge/HL7-FHIR_R4-red?style=flat-square) ![DICOM](https://img.shields.io/badge/DICOM-pydicom-blue?style=flat-square) ![LGPD](https://img.shields.io/badge/Compliance-LGPD_/_HIPAA-purple?style=flat-square) |
| **GenAI & NLP** | ![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square) ![ChromaDB](https://img.shields.io/badge/ChromaDB-Vector_Store-orange?style=flat-square) ![SpaCy](https://img.shields.io/badge/SpaCy-09A3D5?style=flat-square&logo=spacy&logoColor=white) |

</div>

---

## 💼 Why Hire Me? (O Diferencial Competitivo)

### 🇧🇷 Para Empresas e Operadoras no Brasil
Grandes grupos hospitalares e empresas de dados (Einstein, Sírio, Fleury, Dasa, Hapvida, seguradoras e consultorias) frequentemente sofrem com cientistas de dados que desconhecem a rotina clínica e a regulamentação sanitária.
* Eu trago **mais de 10 anos de experiência real em ambientes hospitalares críticos** resolvendo problemas em salas de emergência e centros cirúrgicos.
* Conheço a física do equipamento médico, o fluxo de prontuários eletrônicos e a **LGPD na prática**, implementando microsserviços com segregação física de PII.

### 🌐 For US, European & Global Remote Companies (Hiring in USD/EUR)
Global hiring managers need autonomous, mature engineers who write reliable, maintainable software and communicate transparently.
* **Production-Grade Engineering:** Every single project features modular clean code, strict Pydantic schemas, PyTest automated testing suites, Docker containerization, and automated CI/CD pipelines.
* **International Standards Leadership:** Mastery in **openEHR and HL7 FHIR R4**, which are the required backbone for European and US digital health networks.
* **Multilingual Capability:** Fluent in English for technical architecture and code documentation, with conversational technical German (`thyroid_eda_portfolio_deutsch_val.ipynb`).

---

## 📬 Let's Connect!

I am actively open to discussions regarding **Senior Data Scientist, Machine Learning Engineer, and Healthcare AI Architect** roles.

* 📧 Email: [pauloelias41@gmail.com](mailto:pauloelias41@gmail.com)
* 💼 LinkedIn: [linkedin.com/in/paulo-generozo](https://linkedin.com/in/paulo-generozo)
* 🌐 GitHub Repositories: [github.com/generozo-paulo](https://github.com/generozo-paulo)
* 🔬 R&D Algorithms: [github.com/paulo-generozo](https://github.com/paulo-generozo)

</div>
