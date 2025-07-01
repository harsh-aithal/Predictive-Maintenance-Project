# 🛠️ Predictive Maintenance using Machine Sensor Data

This project aims to predict equipment failures using real-world sensor data from industrial machines. It uses machine learning (Random Forest and XGBoost) to classify failure types based on environmental and mechanical conditions.

---

## 📊 Dataset Summary

- **Total Samples**: 10,000
- **Target Variable**: `Failure Type` (6 categories)
- **Sensor Features**:
  - Air & Process Temperature
  - Rotational Speed
  - Torque
  - Tool Wear
  - Product Type (categorical)

---

## 🧪 Models Used

| Model             | Accuracy | Notes                              |
|------------------|----------|-------------------------------------|
| Random Forest     | 98%      | High accuracy but poor for rare failures |
| **XGBoost (final)** | **99%**  | Best recall + precision on majority + minority classes |

> Rare failures like `Tool Wear Failure` and `Random Failures` are underrepresented and need more samples or data balancing in future work.

---

## 🔍 Feature Importance (from XGBoost)

1. **Torque** — most important  
2. **Tool Wear**  
3. **Air Temperature**  
4. **Rotational Speed**  
5. **Process Temperature**  
6. **Machine Type (L, M)**

---

## 📁 Project Structure
Predictive_Maintenance_Project/
├── data/
├── notebooks/
├── results/
├── README.md
└── requirements.txt
---

## 📦 Tools & Libraries

- Python, Pandas, NumPy, Seaborn, Matplotlib
- Scikit-learn
- XGBoost

---

## 📌 Author

Harsha Aithal  
`IBM Data Science Certified | DA/DS Aspirant | Looking for roles in Germany/India`

---

## 📎 How to Run

```bash
pip install -r requirements.txt
jupyter notebook
