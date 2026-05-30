# Shock Absorber Design & Multiphysics Simulation
 *(Autodesk Inventor + ANSYS Mechanical APDL)*

---

## Project Overview

This project focuses on the **design, modeling, and multiphysics simulation of a mechanical shock absorber**.
The aim was to analyze its real-world behavior under static, modal, and random vibration conditions, using **Autodesk Inventor** for 3D CAD modeling and **ANSYS Mechanical APDL** for finite element analysis (FEA).

---

## Objectives

* Design a **fully functional shock absorber assembly** with adjustable spring tension.
* Perform **static structural analysis** to study stress and deformation under compression.
* Conduct **modal analysis** to identify natural frequencies and avoid resonance.
* Execute **random vibration analysis** using **Power Spectral Density (PSD)** input to simulate dynamic conditions.

---

## CAD Modelling (Autodesk Inventor)

**Components Modeled:**

* Main Rod / Body
* Plunger / Base
* Threaded Nut (for spring tension adjustment)
* Helical Coil Spring

All parts were created as individual `.ipt` files and assembled into a fully constrained `.iam` assembly.

---

## ⚙️ Material Properties

| Component            | Material         |
| -------------------- | ---------------- |
| Spring / Coil        | Structural Steel |
| All Other Components | Gray Cast Iron   |

---

## Simulation Workflow (ANSYS Mechanical APDL)

### 1. **Static Structural Analysis**

* **Applied Load:** Displacement = -10 mm along Y-axis
* **Support:** Fixed base at plunger
* **Results:**

  * Max Deformation: **1.01E-02 m**
  * Max Equivalent Stress (Von Mises): **2.13 GPa**
  * Max Elastic Strain: **1.44E-02 m/m**

---

### 2. **Modal Analysis**

Extracted six natural frequencies:

| Mode | Frequency (Hz) |
| ---- | -------------- |
| 1    | 657.5          |
| 2    | 697.47         |
| 3    | 853.57         |
| 4    | 980.78         |
| 5    | 1152.4         |
| 6    | 1197.8         |

**Inference:** Design ensures sufficient frequency separation to avoid resonance.

---

### 3. **Random Vibration Analysis**

* **Input:** Power Spectral Density (PSD) acceleration from 5 Hz to 50 Hz
* **PSD Data:**

  * 5 Hz → 100 (m/s²)²/Hz
  * 10 Hz → 150 (m/s²)²/Hz
  * 20–30 Hz → 200 (m/s²)²/Hz
  * 50 Hz → 100 (m/s²)²/Hz
* **Outcome:** Structural integrity maintained under dynamic base excitation.

---

## Technical Highlights

* **Contact Types:**

  * Frictional (μ = 0.1 & 0.3)
  * Bonded

* **Mesh Details:**

  * Element Size: 0.003 m
  * Refined mesh at contact and stress concentration regions

---

## Skills & Tools Developed

* **CAD Modeling & Assembly** (Autodesk Inventor)
* **FEA Simulation** (ANSYS Mechanical APDL)
* **Modal & Vibration Analysis**
* **APDL Command Workflow & Solver Understanding**
* **Result Interpretation & Engineering Decision-Making**

---

## Software Used

| Software                       | Purpose                       |
| ------------------------------ | ----------------------------- |
| Autodesk Inventor Professional | 3D Modelling & Assembly       |
| ANSYS Mechanical APDL          | Finite Element Analysis (FEA) |


---


## Mesh and Geometry

---

<img width="1919" height="1027" alt="Ring" src="https://github.com/user-attachments/assets/23ff8c2a-dbda-48a8-8bc4-fff4715bfb3a" />
<img width="1919" height="1029" alt="Plunger" src="https://github.com/user-attachments/assets/1ac8cb49-cc5f-46a2-950e-973c94e66ffe" />
<img width="1919" height="1036" alt="Mesh" src="https://github.com/user-attachments/assets/bf151f3e-d0f6-4468-9b6f-6d8f2795c043" />
<img width="1919" height="1027" alt="Geometry" src="https://github.com/user-attachments/assets/e4482ebc-c02e-42ad-acca-3157ee8d10c7" />
<img width="1919" height="1031" alt="Cylinder" src="https://github.com/user-attachments/assets/17d1cbcc-3111-48c2-be03-a8d3dea503ec" />
<img width="1919" height="1032" alt="Coil" src="https://github.com/user-attachments/assets/7ad0db7c-01af-4867-be6d-41203e887ad3" />
<img width="1919" height="1033" alt="Assembly" src="https://github.com/user-attachments/assets/dc77510c-0b08-449c-b818-016553c95946" />
<img width="1919" height="1032" alt="Contacts4" src="https://github.com/user-attachments/assets/ef8b8bb8-f559-4047-a291-4630438fd128" />
<img width="1919" height="1028" alt="Contacts3" src="https://github.com/user-attachments/assets/16a6fa07-c9e6-412a-a2a9-0321a55d18b1" />
<img width="1919" height="1028" alt="Contacts2" src="https://github.com/user-attachments/assets/919c3f3c-6040-47ce-a4c3-3257ebf5a5e1" />
<img width="1919" height="1036" alt="Contacts1" src="https://github.com/user-attachments/assets/1168eabe-988c-48fe-834b-89503ce7d04b" />
<img width="1919" height="1033" alt="Contacts" src="https://github.com/user-attachments/assets/534fe125-71cb-4fa0-af6e-eaaa6e1ead6a" />


---

## Modal Analysis

---

![Modal(BS)_Total_Deformation](https://github.com/user-attachments/assets/29741352-510a-449e-b32e-ecf190a53bdd)
<img width="1919" height="1034" alt="M_TD" src="https://github.com/user-attachments/assets/0203f004-444a-41c6-8cb4-91d32900ea75" />
![M_TD](https://github.com/user-attachments/assets/eb0a186a-bf5b-471b-a63b-87c2365132b7)


---

## Random Vibrations

---

<img width="1919" height="1033" alt="RV_ES" src="https://github.com/user-attachments/assets/1eaefcf2-77cd-4aef-bec3-4934eb39af06" />
<img width="1919" height="1034" alt="RV_ES!" src="https://github.com/user-attachments/assets/409f94dd-c91f-42b1-80dc-b7ad65d5909c" />
<img width="1919" height="1031" alt="RV_DD_Z" src="https://github.com/user-attachments/assets/8d838618-1a31-4ddf-8475-2f365574b5c5" />
<img width="1919" height="1034" alt="RV_DD_X" src="https://github.com/user-attachments/assets/38bf8639-72ab-40c5-8fe2-4514a2897418" />
<img width="1919" height="1037" alt="RV_DD_V" src="https://github.com/user-attachments/assets/f51b9734-599e-4987-96ee-a712c840fb39" />


---

## Static Structural

---

![TD_SS](https://github.com/user-attachments/assets/21d27e44-7c24-4e8d-8c8c-5a83e453062c)
![ES_SS](https://github.com/user-attachments/assets/257aac75-285e-4b5d-a705-f96d08bf4dc4)
![EES_SS](https://github.com/user-attachments/assets/8a36b326-2a61-4432-8730-25e7f46c24d6)


---


## Key Results Summary

| Parameter             | Value          | Unit |
| --------------------- | -------------- | ---- |
| Max Deformation       | 1.01E-02       | m    |
| Max Equivalent Stress | 2.13E+09       | Pa   |
| Frequency Range       | 657.5 – 1197.8 | Hz   |

---

## 🧾 Conclusion

The **shock absorber model** successfully demonstrates the integration of **CAD and FEA tools** for realistic mechanical analysis.
The **structural and modal results** validate that the design can withstand expected mechanical and vibrational loads without entering resonance or exceeding material limits.
This project deepened understanding of **multiphysics coupling**, **contact mechanics**, and **FEA validation workflows**, making it a valuable reference for future simulation-based design projects.

---


### Author
**Mohammad Haris** — Mechanical Engineer | FEA & CFD Engineer

GitHub: [github.com/MohammadHaris13](https://github.com/MohammadHaris13)

   
[Linkedin Profile](https://linkedin.com/in/mohammad-haris-13032002) | [Email](mailto:mohammaddharis1303@gmail.com)
