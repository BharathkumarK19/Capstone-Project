🚀 End-to-End Machine Learning Pipeline on AWS EKS
📌 Project Overview
This project demonstrates a complete MLOps pipeline — from data ingestion to deployment and monitoring — leveraging AWS services, containerization, CI/CD automation, experiment tracking, and observability tools.
Capstone-project - sentiment Analysis
The workflow covers:

Data ingestion from AWS S3

Data preprocessing & transformation

Model training, evaluation & registry

Experiment tracking with MLflow

Code versioning with Git

Data versioning with DVC

Docker image creation & push to AWS ECR

CI/CD with GitHub Actions

Deployment to AWS EKS

Monitoring & alerting with Prometheus & Grafana

 Architecture
mermaid
Copy
Edit
graph LR
A[📦 AWS S3 - Raw Data] --> B[⚙ Data Ingestion]
B --> C[🧹 Data Preprocessing]
C --> D[🤖 Model Training]
D --> E[📊 Model Evaluation]
E --> F[🧾 Experiment Tracking - MLflow]
F --> G[📜 Model Registry]
G --> H[🐳 Docker Image Build]
H --> I[📤 Push to AWS ECR]
I --> J[🔄 CI/CD - GitHub Actions]
J --> K[☸ Deploy to AWS EKS]
K --> L[📡 Monitoring - Prometheus]
L --> M[📈 Visualization - Grafana]
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Cloud Storage	AWS S3
Version Control	Git + GitHub
Data Versioning	DVC
Experiment Tracking	MLflow
Containerization	Docker
Image Registry	AWS ECR
Orchestration	AWS EKS (Kubernetes)
CI/CD	GitHub Actions
Monitoring	Prometheus + Grafana

------------------------------------------------------------------------->>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

📌 Workflow Steps
1️⃣ Data Ingestion
Fetched raw datasets from AWS S3 bucket.

Stored intermediate & processed datasets with DVC for reproducibility.

2️⃣ Data Preprocessing
Cleaning, handling missing values, encoding, and feature engineering.

3️⃣ Model Training & Evaluation
Implemented training scripts to fit ML models.

Evaluated metrics (accuracy, F1-score, etc.).

4️⃣ Experiment Tracking with MLflow
Tracked hyperparameters, metrics, and artifacts for each run.

Compared experiments to choose the best-performing model.

Integrated MLflow Model Registry to manage model lifecycle stages.

5️⃣ Version Control & Data Versioning
Git for code tracking.

DVC for data & model artifact version control.

6️⃣ Dockerization & AWS ECR
Created Dockerfile to package the application.

Pushed Docker images to AWS ECR.

7️⃣ CI/CD with GitHub Actions
Automated pipeline:

Pull latest code

Build & push Docker image to ECR

Deploy to AWS EKS

8️⃣ AWS EKS Deployment
Kubernetes manifests for deployment & service.

Configured port mapping for public access.

9️⃣ Monitoring & Alerting
Metrics collection with Prometheus.

Dashboard visualization with Grafana.

Alerts configured for failures & performance drops.

------------------------------------------------------------------------------------------------------


✅ Fully automated ML pipeline
✅ Data & model versioning
✅ Experiment tracking with MLflow
✅ Scalable cloud-native deployment
✅ CI/CD with GitHub Actions
✅ Live monitoring & alerting
