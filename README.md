# 📘 Delta Lake with Databricks (Spark-Only Hands-On Guide)

This repository documents a **step-by-step hands-on exploration of Delta Lake using Databricks**, focusing on **Spark-based workflows**, **Unity Catalog**, **Volumes**, **data versioning**, and **safe data modification**.

All concepts are demonstrated using **actual executed code and real outputs**.

---

## 🧠 Objective

- Understand how Delta Lake works internally  
- Learn how Databricks manages storage using Unity Catalog & Volumes  
- Create and modify Delta tables using **Spark only (no SQL dependency)**  
- Observe **data versioning and time travel in action**  
- Build a strong mental model of **how Delta guarantees safety**

---

## 🏗️ Environment Overview (Databricks)

This setup uses **modern Databricks with Unity Catalog enabled**, which enforces:

- Secure storage access  
- Catalog–schema–volume hierarchy  
- No public DBFS root access  

---

## 1️⃣ Exploring Databricks Storage

### Code

```python
dbutils.fs.ls("/")
```
```
Output:
Volumes/
Workspace/
databricks-datasets/
```
