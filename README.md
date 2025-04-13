# 📘 Project Title
**Experimental and Numerical Investigation of Open-Cycle Miniature Joule-Thomson Cryocooler for Working Temperatures 100 K to 150 K with Single Component Coolants**

---

## 👨‍🔬 Author

**Siddharth Verma**  
Roll No: 22B2153  
Course: ME-683 | Cryogenic Engineering  

---

## 📌 Abstract

This project investigates the performance of an **open-cycle miniature Joule-Thomson (JT) cryocooler** using **single-component coolants** such as **Krypton**, **R14**, and **Nitrogen Trifluoride (NF₃)** in the temperature range of **100 K to 150 K**. Both **experimental and theoretical analyses** were performed, with additional simulations proposed using **Physics-Informed Neural Networks (PINNs)**.

> All thermophysical property data used for the analysis, including enthalpy, boiling points, and pressure relationships, were sourced from the **NIST REFPROP database**.

---

## 🧊 Application Areas

- Cryosurgery  
- Infrared Detectors (HOT detectors operating at 130K–175K)  
- Liquefaction of Natural Gas  
- Missile Guidance Systems  

---

## 🔍 Background and Motivation

Most prior work focuses on **multi-component mixtures** in **closed-cycle configurations**, which increases system complexity and instability. This project explores the **simpler alternative**: **open-cycle systems with single-component coolants**, ideal for portable, low-maintenance applications.

---

## 🔬 Methodology

### Experimental Setup:
- Cryocooler connected to a pressure vessel filled with either **Krypton** or **R14**
- Ambient temperature settings: **293 K and 343 K**
- Key Performance Metrics:
  - **Cool Down Time (CDT)**
  - **Cooling Duration Period (CDP)**
  - **Cutoff Pressure (CP)**

### Theoretical Analysis:
- NTU (Number of Transfer Units) approach applied to a **recuperative finned-tube heat exchanger**
- Key variables: **mass flow rate**, **isothermal effect**, and **heat exchanger efficiency**
- Governing equation:  
  \[
  Q_{\text{cooling}} = \text{NTU} \times \dot{m} \times \Delta h_{\text{JT}}
  \]

---

## 📊 Experimental Results Summary

| Coolant | Ambient Temp | CDT (s) | CDP (s) | Cutoff Pressure (MPa) |
|---------|---------------|---------|---------|------------------------|
| Krypton | 293 K         | 3.0     | 160     | 0.93                   |
| R14     | 293 K         | 3.8     | 146     | 1.77                   |
| Krypton | 343 K         | 5.6     | —       | 1.32                   |
| R14     | 343 K         | 7.6     | —       | 5.10                   |

---

## 📈 Theoretical Comparison Using NIST Data

The **enthalpy drop (Δh)** is the most important parameter for JT cooling efficiency. NIST data shows:

| Coolant | Δh @ 293.15K (J/kg) | Δh @ 343.15K (J/kg) |
|---------|----------------------|----------------------|
| **NF₃**     | 88,223               | **122,293**            |
| Krypton | 55,240               | 44,964               |
| R14     | 66,577               | 53,998               |

> 🔍 **NF₃ shows a unique increase in Δh with temperature**, unlike Krypton and R14, making it a superior candidate for HOT detectors.

---

## 💡 Why NF₃?

After evaluating over a dozen compounds (boiling points, flammability, toxicity, etc.), **NF₃ (Nitrogen Trifluoride)** was identified as the **most suitable refrigerant**:

- **Boiling Point ~144 K** — perfect for the 100–150 K range  
- **Non-flammable and chemically stable**  
- **Higher enthalpy drops at elevated temperatures**  
- **Simple single-component behavior, no pinch points**  
- **Safe for open-cycle systems (unlike flammable hydrocarbons)**  

All its thermophysical properties were obtained from the **NIST REFPROP database**.

---

## 📐 Effective Cooling Power

From NIST data at 343.15 K, using the equation:  
\[
\Delta h = \frac{h_{\text{low-pressure}} - h_{\text{high-pressure}}}{M}
\]

NF₃ outperforms both R14 and Krypton across all operating pressures.  
This makes NF₃ an ideal coolant for portable cryocoolers operating in **unregulated open-cycle environments**.

---

## 🔮 Future Work

### 🧠 PINNs for Cryocooler Simulation
To replace complex numerical solvers, we plan to use **Physics-Informed Neural Networks (PINNs)** to:

- Solve governing PDEs of heat transfer and mass flow
- Model enthalpy-pressure-temperature behavior directly from NIST data
- Simulate JT cooling curves for varying ambient temperatures
- Predict cooling behavior for other candidate refrigerants

---

## 🧾 Repository Structure

