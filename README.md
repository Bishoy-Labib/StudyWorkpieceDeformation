# Investigation of Workpiece Deformation in CNC Clamping

## 📖 Research Context
In high-precision manufacturing, particularly for medical devices, the geometric accuracy of the final product is paramount. [cite_start]A critical but often overlooked source of error is the elastic deformation of the workpiece caused by clamping forces[cite: 127]. [cite_start]This research investigates the **"convex phenomenon"**—a geometric error where a workpiece machined flat under load springs back to a convex shape upon release[cite: 47, 132].

[cite_start]The primary objective was to quantify this deformation using analytical, experimental, and numerical methods to determine ideal clamping parameters that minimize geometric inaccuracies[cite: 47, 127].

## 🔬 Methodology
To comprehensively analyze the deformation behavior, the study triangulated data from three distinct approaches:

### 1. Analytical Approach
[cite_start]The theoretical clamping force applied by the vise was calculated based on input torque[cite: 46]. [cite_start]Using the mechanics of the **Gerardi StandardFLEX vise** (TR24x5 trapezoidal thread), we established the relationship between the applied torque and the resulting linear force exerted on the workpiece[cite: 696, 697, 721].

### 2. Experimental Metrology (CMM)
[cite_start]Physical experiments were conducted using **Aluminum alloy 6082 (AlMgSi1)** bars of varying dimensions (20x20mm and 40x40mm)[cite: 714].
* [cite_start]**Setup:** A **COORD3 Universal CMM** equipped with a **Renishaw SP25M** scanning probe was utilized to map the surface topology[cite: 730, 733].
* [cite_start]**Procedure:** Measurements were taken at incremental clamping torques ranging from 0 Nm to 100 Nm to track surface deviation[cite: 754].

![CMM Measurement Setup](path/to/image.jpg)
### 3. Finite Element Analysis (FEM)
[cite_start]A "Digital Twin" of the setup was created in **ANSYS** to simulate the elastic behavior[cite: 145].
* [cite_start]**Model:** The vise jaw was treated as a rigid body, while the workpiece was modeled as a flexible body with a Young's Modulus of 70 GPa[cite: 801, 804].
* [cite_start]**Mesh:** A tetrahedral mesh with 3mm sizing was applied to balance computational efficiency with accuracy[cite: 805].

![FEM Mesh Setup](path/to/image.jpg)
## 📊 Key Findings
Data processing in **MATLAB** revealed significant insights regarding the behavior of the material under load:

* [cite_start]**Convex Deformation:** As hypothesized, higher clamping torques resulted in a measurable convex profile on the machined surface[cite: 789].
* [cite_start]**Z-Axis Translation:** The empirical data revealed a consistent vertical translation (lifting) of the workpiece, averaging approximately **0.03 mm per 10 Nm** of applied torque[cite: 796, 799]. [cite_start]This suggests that the moving jaw of the vise contributes a translational error vector that must be accounted for[cite: 1084].
* [cite_start]**Simulation Validation:** The ANSYS simulation results correlated closely with the physical CMM measurements regarding deformation magnitude, validating the FEM model for predictive analysis[cite: 820].

![Deformation Heatmap](path/to/image.jpg)
## 🛠️ Technical Specifications
* [cite_start]**Metrology:** COORD3 Universal CMM, TouchDMIS software[cite: 730].
* [cite_start]**Simulation:** ANSYS (Parametric function)[cite: 815].
* [cite_start]**Material:** AlMgSi1 (Aluminum 6082)[cite: 714].
* [cite_start]**Fixture:** Gerardi StandardFLEX Vise[cite: 721].

---
[cite_start]*Based on the Master's Thesis: "Optimization of medical device manufacturing technology" by Bishoy Labib (2025)[cite: 1].*
