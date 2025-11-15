# 🔍 Kubernetes Intelligent Log Analysis using MLOps  
### AIOps Project — Log Anomaly Detection on Kubernetes using Loki, Kubeflow & ML  
#### By **Arbind Kr. Mahato — AWS Cloud | DevOps | MLOps Engineer**

---

## 📌 Project Summary

This project implements **automated log anomaly detection** on Kubernetes using:

- **Kubernetes (EKS / Kind / Kubeadm)**
- **Loki (log collection)**
- **Kubeflow Pipelines (ML automation)**
- **Machine Learning anomaly detection models**
- **Prometheus + Grafana dashboards**
- **Slack/Email alerting (optional)**

It is designed to showcase real-world **AIOps capabilities**, enabling automatic detection of abnormal patterns in cluster logs—helping DevOps teams catch issues early.

This project is a part of my MLOps portfolio inside the repository **MLOps-Project-Library**.

---

# 🚀 Why This Project Matters

Modern applications generate millions of logs.  
Manually detecting issues such as:

- Sudden spike in errors  
- Unknown failure patterns  
- CrashLoopBackOff anomalies  
- Unauthorized API calls  
- Application exceptions  
- Network or storage disruptions  

…is nearly impossible.

This project solves that challenge using **Machine Learning** trained on Kubernetes logs.

### ✔ Business & Operational Impact

- **Detect incidents before they break production**
- **Reduce MTTR (Mean Time to Recovery)**
- **Identify hidden or unknown errors using ML**
- **Spot unusual patterns (DoS, retries, auth failures)**
- **Improve overall reliability of Kubernetes workloads**
- **Create a practical AIOps engine for DevOps teams**

---

# 🧠 Architecture

          ┌───────────────┐
          │ Kubernetes     │
          │ Pods / Nodes   │
          └───────┬────────┘
                  │ Logs
                  ▼
         ┌──────────────────┐
         │ Loki (Log Store) │
         └───────┬──────────┘
                 │ Pull Logs
                 ▼
    ┌────────────────────────────┐
    │ Kubeflow Pipeline (ML)     │
    │ - Preprocessing            │
    │ - Vectorization            │
    │ - Model Training           │
    │ - Prediction Pipeline      │
    └─────────┬──────────────────┘
              │ Output
              ▼
    ┌────────────────────┐
    │ ML Model Output     │
    │ - Normal / Anomaly  │
    └─────────┬───────────┘
              │
              ▼
    ┌────────────────────────────┐
    │ Grafana Dashboard          │
    │ Prometheus Metrics         │
    └────────────────────────────┘


---

# 🧩 Key Features

### ✅ 1. **Automated Log Collector**  
Using **Loki**, logs from pods, nodes, and applications are streamed for analysis.

### ✅ 2. **Feature Engineering on Logs**  
Logs are cleaned, tokenized, vectorized using:

- TF-IDF  
- Word embeddings  
- Count vectorization  

### ✅ 3. **Machine Learning Model**  
ML algorithms used:

- Isolation Forest  
- Autoencoder (optional)  
- One-Class SVM  

### ✅ 4. **Kubeflow Orchestrated Pipeline**  
Kubeflow automated stages:

- Download Loki logs  
- Preprocess logs  
- Train anomaly detection model  
- Evaluate & generate anomaly score  
- Store model artifacts  
- Trigger inference pipeline  

### ✅ 5. **Grafana Visualization**  
Live metrics:

- Error spikes  
- Number of anomalies per pod  
- Time-series anomaly detection  
- Pod-specific anomaly levels  

### ✅ 6. **Alerting (Optional)**  
Send alerts via:

- Slack  
- Email  
- PagerDuty  
- Teams  

---

# 📁 Project Structure

k8-intelligent-log-analysis-mlops/
│

├── pipeline/

│ ├── anomaly_pipeline.py

│ ├── preprocessing.py

│ ├── training.py

│ ├── inference.py

│ └── components/

│

├── manifests/

│ ├── loki/

│ ├── grafana/

│ ├── kubeflow/

│ └── RBAC/

│

├── dataset/

│ └── sample-loki-logs.json

│

├── notebooks/

│ ├── eda.ipynb

│ ├── model-dev.ipynb

│

├── dashboard/

│ └── grafana-json/

│

└── README.md ← (You are reading this file)



---

# 🛠 Tools & Technologies

### **DevOps / Kubernetes**
- Kubernetes / EKS / Kind  
- Loki, Promtail  
- Prometheus  
- Grafana  

### **MLOps / ML**
- Kubeflow Pipelines  
- Python  
- Scikit-learn  
- TensorFlow Autoencoders (optional)  
- Pandas / NumPy  

### **Other**
- Docker  
- GitHub Actions CI/CD  
- MinIO (optional S3)  

---

# 🚀 How the Pipeline Works (Step-by-Step)

### **1️⃣ Pull Logs from Loki**
Kubeflow component fetches logs via REST API.

### **2️⃣ Clean & Transform**
Logs go through preprocessing pipeline:

- Remove timestamps  
- Tokenize  
- Filter noise  
- Convert text → numerical vectors  

### **3️⃣ Train Model**
Isolation Forest identifies abnormal sequences.

### **4️⃣ Evaluate & Save Artifacts**
Artifacts stored in:

- MinIO  
- S3  
- Local persistent volume  

### **5️⃣ Inference Pipeline**
New logs are streamed → model predicts:

✔ Normal  
❌ Anomaly  

### **6️⃣ Grafana Dashboard Visualization**
Results appear as:

- Time series charts  
- Anomaly scores  
- Pod-level grouping  

---

# 🧪 Sample Output

- **Anomaly Score:** 0.89  
- **Pod Identified:** `payment-service-7dbf4c`  
- **Category:** Unusual Error Pattern  
- **Suggested Action:** Review API latency & DB connections  

---

# 🌟 Why This Project Is Impressive (For Your Boss)

✔ Shows your capability of integrating **DevOps + MLOps + AIOps**  
✔ Works on real Kubernetes logs — not dummy datasets  
✔ Demonstrates automation, monitoring, ML, pipelines, and visualization  
✔ Can be converted into a company-wide internal AIOps platform  
✔ Reduces operational noise and improves stability  

---

# 📬 Connect With Me  

**👨‍💼 Arbind Kr. Mahato**  
AWS Cloud | DevOps | MLOps Practitioner  
- 🔗 LinkedIn: https://www.linkedin.com/in/arbindmahato/  
- ▶️ YouTube: https://www.youtube.com/techmahato  
- 🎥 Vlog Channel: https://youtube.com/@TechMahatoVlogs?sub_confirmation=1  
- 📸 Instagram: https://instagram.com/techmahato  
- 🌐 Website: https://techmahato.com  

---

# ⭐ Support This Project

If you find this project useful, please ⭐ star the repository in GitHub.  
Your support motivates me to build more real-world MLOps projects!

