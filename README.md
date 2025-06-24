# 🚀 System Log Classification using Hybrid AI and FastAPI (CS/ML Integrated System
This project implements a hybrid log classification system, combining **traditional rule-based methods, machine learning, and Generative AI** for **accurate and scalable log analysis**.  

---

## 🛠 Classification Framework  
1️⃣ **Regex-Based Classification** → Handles predictable, rule-based patterns.  
2️⃣ **Sentence Transformer + Logistic Regression** → Learns from structured labeled data.  
3️⃣ **Large Language Models (LLM - DeepSeek R1, BERT)** → Handles complex and low-resource scenarios.  

This hybrid approach ensures flexibility in **processing structured, semi-structured, and unstructured logs**.  

---

## 📂 Project Structure  
📁 **training/** → Model training (Sentence Transformer, Logistic Regression, Regex).  
📁 **models/** → Pretrained classification models.  
📁 **resources/** → Sample datasets, log files, output predictions, and architecture diagram.  
📁 **Root Directory** → Contains `server.py` (FastAPI backend for log classification API).  

---

## ⚙️ Installation & Setup  
### **Step 1: Install Dependencies**  
```bash
pip install -r requirements.txt


Step 2: Run FastAPI Server
uvicorn server:app --reload

Step 3: Access API & Test Classification
🌐 Swagger UI: http://127.0.0.1:8000/docs

📂 Upload CSV file with logs (source, log_message) → Get classified logs (target_label).

📌 Usage
1️⃣ Prepare a CSV file with the following columns:
      source,  log_message
2️⃣ Upload the file using the API or a script.
3️⃣ The system will classify logs and return an updated CSV with target_label.

📌 Designed for scalable and accurate log classification! 🚀

