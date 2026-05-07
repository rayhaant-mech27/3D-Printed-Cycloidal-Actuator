# 3D-Printed PETG Cycloidal Actuator (19:1)

## Project Overview
[cite_start]This project involves the design, prototyping, and performance analysis of a high-reduction cycloidal drive fabricated using PETG material via FDM 3D printing[cite: 49, 85]. [cite_start]Cycloidal drives offer significant advantages in robotics, such as high reduction ratios in a single stage and very low backlash[cite: 50, 81]. [cite_start]This research specifically investigates the feasibility of using PETG for functional mechanical actuators[cite: 51, 128].

---

## Design Specifications
[cite_start]The actuator was modeled in SolidWorks with a profile generated via parametric equations[cite: 261, 309].

* [cite_start]**Theoretical Reduction Ratio:** 19:1[cite: 198, 237].
* [cite_start]**Eccentricity ($E$):** 2.0 mm[cite: 204].
* [cite_start]**Ring Pin Radius ($R$):** 40.0 mm[cite: 207].
* [cite_start]**Number of Ring Pins ($Z_r$):** 20[cite: 209].
* **Number of Cycloidal Lobes ($Z_d$):** 19[cite: 212].
* **Housing Dimensions:** 80 mm Diameter x 40 mm Height[cite: 198].

---

## Fabrication & Materials
The components were fabricated using **PETG (Polyethylene Terephthalate Glycol)**, selected for its superior strength-to-flexibility ratio and low warping compared to PLA and ABS[cite: 86, 184].

* [cite_start]**Infill Density:** 100%[cite: 342].
* [cite_start]**Infill Pattern:** Gyroid (for isotropic strength)[cite: 342].
* **Layer Height:** 0.16 mm[cite: 342].
* [cite_start]**Wall Count:** 4[cite: 342].
* [cite_start]**Standard Parts:** Integrated 6202 deep groove ball bearings for the eccentric input shaft[cite: 302, 352].

---

## Performance Analysis & Experimental Results
[cite_start]The actuator underwent systematic testing using a NEMA 17 stepper motor and a custom test rig to verify its mechanical properties[cite: 370, 386].

| Metric | Measured Value | Ideal/Target |
| :--- | :--- | :--- |
| **Reduction Ratio** | [cite_start]18.99:1 [cite: 680] | [cite_start]19:1 [cite: 237] |
| **Peak Output Torque** | [cite_start]5.28 Nm [cite: 56, 521] | [cite_start]11.0 Nm (Theoretical) [cite: 259] |
| **Max Efficiency** | [cite_start]61.8% (at light load) [cite: 57, 522] | [cite_start]65% (Assumed) [cite: 256] |
| **Backlash** | [cite_start]0.24° [cite: 58, 502] | [cite_start]< 0.5° [cite: 105] |

### Key Observations:
* [cite_start]**Precision:** The kinematic verification showed near-perfect agreement with the theoretical reduction ratio, confirming the accuracy of FDM-printed cycloidal geometry[cite: 425, 520].
* **Backlash:** At 0.24°, the precision is comparable to industrial harmonic drives and vastly superior to standard spur gears[cite: 502, 523].
* [cite_start]**Failure Mode:** Testing revealed that progressive plastic deformation of the cycloidal disc lobes is the dominant failure mode at input torques above 1.4 Nm[cite: 512, 526].

---

## Repository Structure
* `/CAD`: .STEP files for assembly and .STL files for printing.
* `/Calculations`: MATLAB scripts for cycloidal profile generation.
* `/Docs`: Full Mini-Project report and technical presentation.
* `/Media`: Demo videos and high-res assembly photos.

---

## Future Scope
* [cite_start]Investigating **Carbon Fiber reinforced PETG** for higher stiffness and torque capacity[cite: 540, 708].
* Integrating **metal sleeves/inserts** at high-stress contact points to mitigate lobe deformation[cite: 545, 710].
* [cite_start]Implementation of **active cooling** schemes for high-load operations[cite: 553, 712].