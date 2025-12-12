# GearFatigue-TCM: Thermographic Estimation of Gear Fatigue Limits

> **A theoretical and experimental framework for estimating the fatigue limit of C45 steel gears using the Two Curves Method (TCM) based on infrared thermography.**

![Status](https://img.shields.io/badge/Status-Completed-success)
![Language](https://img.shields.io/badge/Language-MATLAB-blue)
![Subject](https://img.shields.io/badge/Subject-Mechanical%20Engineering-orange)

## 📖 Project Overview

[cite_start]This project investigates the fatigue behavior of **C45 steel gears**, focusing on the estimation of the fatigue limit using the **Two Curves Method (TCM)**—an innovative methodology based on thermographic analysis[cite: 15]. [cite_start]The study compares the fatigue response of untreated gears against induction-hardened gears to evaluate the impact of surface treatments on mechanical resistance[cite: 17].

[cite_start]The primary objective is to validate TCM as a rapid, non-destructive alternative to traditional statistical methods (such as the Stair-Case method) for detecting the transition between unlimited and limited fatigue life[cite: 16, 21].

## ⚙️ Methodology

[cite_start]The research utilizes a variant of the **European Single Tooth Bending Fatigue (STBF)** test (Wildhaber measurement configuration)[cite: 17, 375].

### The Two Curves Method (TCM)
The fatigue limit is estimated by analyzing thermal parameters extracted from infrared thermography data. Two regression approaches were compared:
1.  [cite_start]**Original TCM:** Linear-Linear regression (for data near the fatigue limit)[cite: 16, 265].
2.  [cite_start]**Modified TCM:** Parabola-Power Law regression (for broader data ranges)[cite: 16, 286].

### Thermal Parameters Analyzed
* [cite_start]**$\Delta T_{temp}$**: The temperature difference between the gear root and a reference specimen[cite: 18, 527].
* **$A_{term}$**: The area subtended by the temperature-time curve[cite: 18, 528].

## 🧪 Experimental Setup

* **Testing Machine:** Amsler 10HFP 422 Vibrophore (Frequency ~145 Hz)[cite: 17, 392].
* [cite_start]**Imaging:** IR Technology Timage XT Infrared Camera (Acquisition at 0.1 Hz)[cite: 413, 418].
* **Specimens:**
    * [cite_start]C45 Steel Gears (Module = 3mm).
    * Condition A: Untreated (Base material).
    * [cite_start]Condition B: Induction Hardened[cite: 390].
* [cite_start]**Processing:** Data extraction and processing via MATLAB scripts[cite: 425].

## 📊 Key Results

| Material Condition | Parameter Used | Estimated Limit $\sigma_{FP}$ | ISO 6336 Reference | Error % |
| :--- | :--- | :--- | :--- | :--- |
| **C45 Base** | $\Delta T_{temp}$ | 598 MPa | 555 MPa | +7.7% |
| **C45 Base** | $A_{term}$ | 582 MPa | 555 MPa | +4.8% |
| **C45 Hardened** | Original TCM | 748 MPa | 934 MPa* | -19.9% |
| **C45 Hardened** | Modified TCM | 739 MPa | 934 MPa* | -20.8% |

> [cite_start]*Note on Hardened Results: The discrepancy in the hardened gears is attributed to the specific depth of the industrial hardening treatment applied, which did not fully reach the tooth root fillet as theoretically assumed in the ISO calculation[cite: 834, 835].*

**Conclusions:**
1.  [cite_start]TCM provides a **rapid and accurate estimation** of the fatigue limit for base materials, with errors < 7% compared to ISO standards[cite: 832].
2.  [cite_start]The parameter **$A_{term}$ (Area under curve)** proved more robust and reliable than simple temperature increments[cite: 744].
3.  The methodology successfully identifies the transition point between infinite and finite life[cite: 18].

