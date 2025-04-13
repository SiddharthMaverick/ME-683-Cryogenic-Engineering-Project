# 📘 Project Title
**Experimental and Numerical Investigation of an Open-Cycle Miniature Joule-Thomson Cryocooler for Working Temperatures 100 K to 150 K with Single Component Coolants**

---

## 👨‍🔬 Author
**Siddharth Verma**  
ME-683 | Cryogenic Engineering  
Roll No: 22B2153

---

## 📌 Abstract

This project explores the design, performance, and simulation of an **Open-Cycle Miniature Joule-Thomson (JT) Cryocooler** using **single-component coolants**, primarily **Krypton** and **R14**, operating within the temperature range of **100 K to 150 K**. Theoretical analysis, supported by experimental results, is presented along with a future direction using **PINNs (Physics-Informed Neural Networks)** for simulation of JT cooling behavior.

---

## 🎯 Objective

To experimentally and numerically investigate the performance of an **open-cycle JT cryocooler** using **Krypton and R14** as coolants, and to identify a potentially better-performing candidate such as **Nitrogen Trifluoride (NF₃)**.

---

## 🧊 Applications of JT Cryocoolers

- Cryosurgery  
- Liquefaction of natural gas  
- Cooling of infrared detectors in missile guidance systems  
- Modern HOT IR detectors (130K to 175K)

---

## 🔍 Literature Review Highlights

- **R14**: Previously used in multi-stage cascade coolers.
- **Nitrogen-hydrocarbon mixtures**: Offered stable performance but often flammable or complex.
- **Krypton-R14 binary mix**: Analyzed analytically for <150K cooling.
- **Challenges**: Stability, flammability, complexity, and compatibility with HOT detectors.

---

## 🔬 Current Work

- **Coolant Selection**: Based on boiling/freezing points, REFPROP data, and thermodynamic properties.
- **Focus**: Single-component coolants (Krypton, R14) for open-cycle configurations.
- **Performance Metrics**:
  - Cool Down Time (CDT)
  - Cooling Duration Period (CDP)
  - Cutoff Pressure (CP)

---

## ⚗️ Methodology

- Theoretical calculations focus on the **recuperative heat exchanger** using NTU analysis.
- **Experimental Setup**:
  - Cryocooler in environmental chamber
  - Pressure vessel filled with coolant
  - Tests at 293 K and 343 K ambient conditions

---

## 🧠 Theoretical Results

- **Heat Exchanger Efficiency**:
  - Krypton NTU ≈ 0.94
  - R14 NTU ≈ 0.85
- **Performance Drivers**:
  - Though R14 has a higher isothermal effect, Krypton's higher mass flow rate makes it more effective.

---

## 🧪 Experimental Results

| Ambient Temp | Coolant | Cool Down Time | Cooling Duration | Cutoff Pressure |
|--------------|---------|----------------|------------------|-----------------|
| 293 K        | Krypton | 3.0 s          | 160 s            | 0.93 MPa        |
|              | R14     | 3.8 s          | 146 s            | 1.77 MPa        |
| 343 K        | Krypton | 5.6 s          | -                | 1.32 MPa        |
|              | R14     | 7.6 s          | -                | 5.10 MPa        |

---

## 📈 Effective Cooling Power

Analyzed via enthalpy drops from NIST data:

| Coolant | Δh (J/kg) @ 293 K | Δh (J/kg) @ 343 K |
|---------|--------------------|--------------------|
| NF₃     | 88,223             | **122,293**        |
| Krypton | 55,240             | 44,964             |
| R14     | 66,577             | 53,998             |

> 🔥 NF₃ shows superior performance, with a **Δh increase** at higher temperatures, unlike Krypton or R14.

---

## ✅ Conclusion

- **Krypton**: Shorter Cool Down Time and better cooling duration than R14.
- **NF₃**: Identified as a **superior coolant** for the 100–150K range due to:
  - Favorable boiling point (~144 K)
  - Non-flammability
  - Higher enthalpy drops with temperature

---

## 🌱 Future Work

- **Explore additional candidates**: Noble gases, halides, fluorides
- **Environmental impact**: Evaluate emissions of NF₃
- **Simulations using PINNs**:
  - Train physics-informed neural networks using governing PDEs for heat transfer and fluid dynamics
  - Use experimental boundary conditions and physical constraints for more accurate modeling
  - Replace computationally expensive solvers with neural approximators

---

## 📂 Repository Structure

