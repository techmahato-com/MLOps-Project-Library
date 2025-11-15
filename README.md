# 🚀 MLOps Project Library  
### Production-Grade MLOps & AIOps Projects on Kubernetes, Kubeflow, AWS & GitHub Actions  
#### Created by **Arbind Kr. Mahato — AWS Cloud & DevOps Engineer**

---

## 📌 About This Repository

**MLOps Project Library** is a premium, curated collection of **hands-on, real-world MLOps and AIOps projects** built using:

- **Kubernetes (EKS + KIND)**
- **Kubeflow Pipelines**
- **Prometheus, Grafana, Loki**
- **AWS Cloud Services**
- **GitHub Actions / CI-CD**
- **Python ML frameworks (Sklearn, PyTorch, TensorFlow)**

This repo demonstrates how a DevOps Engineer can evolve into a **full-cycle MLOps Engineer**, building automated pipelines, scalable deployments, intelligent monitoring, and AIOps-driven operational intelligence.

> 📌 **Mission:** To showcase practical, production-ready MLOps projects that solve real business & DevOps problems — not theoretical demos.

---

## 🎯 Why This Repository Exists

I created this library to:

- Transform my DevOps expertise into **MLOps + AIOps capabilities**  
- Build **end-to-end ML pipelines** with automation, monitoring & observability  
- Develop **real POCs** that can be presented to leadership & customers  
- Prepare for **future ML-driven DevOps (AIOps)** roles  
- Help engineers learn **complete production workflows** step-by-step  
- Create a **central knowledge + project hub** under the TechMahato brand  

---

## 🧠 Who Is This Repository For?

This repo is built specially for:

- DevOps Engineers transitioning into MLOps  
- SREs adopting AIOps & automation  
- ML Engineers building scalable pipelines  
- Cloud Engineers exploring Kubeflow/EKS  
- Anyone preparing for MLOps interviews & real projects  
- Companies looking for intelligent automation solutions  

---

# 🏗 Repository Structure
MLOps-Project-Library/
│
├── project-1-intelligent-log-anomaly-detection/
│ ├── src/
│ ├── kubeflow/
│ ├── manifests/
│ ├── notebooks/
│ └── README.md
│
├── project-2-ml-training-cicd/
│ ├── github-actions/
│ ├── pipeline/
│ ├── src/
│ └── README.md
│
├── project-3-ml-observability-stack/
│ ├── prometheus/
│ ├── grafana/
│ ├── loki/
│ └── README.md
│
├── project-4-kserve-real-time-inference/
│ ├── manifests/
│ ├── models/
│ └── README.md
│
└── docs/
├── architecture-diagrams/
├── screenshots/
└── notes/



---

# 🧩 Included Projects (High-Impact)

## **1️⃣ AIOps: Intelligent Log Anomaly Detection (Loki + Kubeflow + ML)**  
📌 **Problem Solved**: Detect production issues BEFORE users complain.  
📌 **Impact**: Reduces outage time, speeds MTTR, detects unknown failures.  
📌 **Components**:  
- Loki log ingestion  
- Pipeline for training anomaly models  
- Isolation Forest / Autoencoder  
- Real-time inference pipeline  
- Alerting via Grafana/Slack  

---

## **2️⃣ CI/CD for ML Training & Deployment (GitHub Actions + Kubeflow)**  
📌 Automates the entire ML lifecycle, including:  
- Dataset validation  
- Model training  
- Testing  
- Deployment to KServe  
- Automated retraining triggers  

---

## **3️⃣ ML Observability Stack (Prometheus + Grafana + Loki)**  
Includes dashboards to monitor:  
- Model latency  
- Accuracy & drift  
- Resource usage  
- Logs, traces & errors  
- End-to-end ML pipeline health  

---

## **4️⃣ Real-Time Inference with KServe (EKS)**  
- Auto-scaling inference  
- Canary rollout support  
- Built-in explainer models  
- Fast, GPU-ready serving  

---

# 🧰 Tech Stack

### **MLOps Tools**
- Kubeflow Pipelines  
- MLflow  
- KServe  
- DVC  

### **DevOps Tools**
- Kubernetes (EKS + KIND)  
- GitHub Actions  
- Terraform  
- Docker  

### **AIOps + Observability**
- Prometheus  
- Grafana  
- Loki  
- Alertmanager  

### **Cloud**
- AWS EKS  
- S3 / ECR / CloudWatch  
- IAM  

---

# 📊 High-Level Architecture
    ┌──────────────────────┐
    │     GitHub Actions   │
    │  CI/CD for ML & Ops  │
    └──────────┬───────────┘
               │
               ▼
    ┌──────────────────────┐
    │  Kubeflow Pipelines  │
    │ Training + Inference │
    └──────────┬───────────┘
               │
               ▼
    ┌──────────────────────┐
    │     Model Registry   │
    │   S3 / MLflow / FS   │
    └──────────┬───────────┘
               │
               ▼
    ┌──────────────────────┐
    │  KServe / Inference  │
    │   Real-Time Serving   │
    └──────────┬───────────┘
               │
               ▼
 ┌─────────────┴─────────────────────────┐
 │ Observability: Prometheus / Grafana    │
 │ Logs: Loki / Alertmanager / Dashboards │
 └────────────────────────────────────────┘



---

# 🏆 My Professional Goals With This Repo

✔ Build enterprise-level MLOps skills  
✔ Deliver impactful AIOps POCs for leadership  
✔ Become a hybrid **DevOps + MLOps + AIOps Engineer**  
✔ Document my complete learning journey  
✔ Create reusable project templates for others  
✔ Grow the **TechMahato** brand through open-source  

---

# 🤝 Contributions

Contributions are welcome!  
If you want to add a new MLOps project or AIOps idea — feel free to open an issue or PR.

---

# 📬 Connect With Me

**👨‍💻 Arbind Kr. Mahato**  
AWS Cloud & DevOps Engineer • MLOps Learner • AIOps Enthusiast  

🔗 **LinkedIn** — https://www.linkedin.com/in/arbindmahato/  
▶️ **YouTube (TechMahato)** — https://www.youtube.com/techmahato  
📸 **Instagram** — https://instagram.com/techmahato  
🌐 **Website** — https://techmahato.com  
🎥 **Vlogs Channel** — https://youtube.com/@TechMahatoVlogs?sub_confirmation=1  

---

# ⭐ Support

If this repo adds value, please ⭐ star it —  
Your support helps grow the **TechMahato** open-source ecosystem!






