# Maritime Logistics Optimization (Berth Scheduling)

This project formulates and solves the **berth scheduling problem** as a **Mixed-Integer Linear Programming (MILP)** model.  
It was developed as a **course project for Operations Research II**, focusing on **ship–berth assignment, sequencing, and service-level optimization** using **Pyomo** and **Gurobi**.

---

## 🧭 Overview
The model assigns ships to berths and determines their service order to minimize total operational cost, considering:
- Berth capacity and extra capacity usage  
- Ship sequencing and precedence constraints  
- Waiting-time penalties and service-level thresholds  
- Sensitivity analysis on berth capacity and service-level parameters  

---

## ⚙️ Implementation
Two formulations were developed:
1. **Pyomo-based MILP model** (Python)
2. **Gurobi direct implementation**

**Key components**
- **Variables:** Assignment (`x`), sequencing (`y`), waiting times (`W`), and binary penalty indicators (`δ₁`, `δ₂`)  
- **Objective:** Minimize total unloading, capacity, and waiting-time costs  
- **Constraints:** Capacity, sequencing logic, and waiting-time thresholds  

---

## 📊 Sensitivity Analysis
The sensitivity analysis investigates the effect of changing **berth capacity** and **service-level thresholds** on:
- Total operational cost  
- Average ship waiting time  
- Berth utilization  

---

## 🧩 Dependencies
- Python 3.x  
- Pyomo  
- Gurobi  
- Pandas  
- NumPy  
- OpenPyXL  

Install dependencies with:
```bash
pip install pyomo gurobipy pandas numpy openpyxl

