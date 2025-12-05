# Single-Stage Cylindrical Gear Reducer (Helical)

> **Status:** Completed Engineering Design
> **Type:** Mechanical Transmission (Helical Gears / Dinți înclinați)

## Project Overview
This repository contains the complete engineering design and analysis of a **single-stage cylindrical gear reducer** utilizing helical gears.

The mechanism is designed to transmit power from an electric motor to a machine load with a fixed reduction ratio of **6.3**, ensuring smooth operation and higher load capacity compared to spur gears due to the $20^\circ$ helix angle.

## Technical Specifications

### Input Parameters
The design is driven by the following requirements:

| Parameter | Symbol | Value | Unit |
| :--- | :---: | :---: | :---: |
| **Required Power** | $P_{load}$ | 2.0 | kW |
| **Input Speed** | $n_1$ | 750 | rpm |
| **Transmission Ratio** | $i$ | 6.3 | - |
| **Helix Angle** | $\beta$ | 20 | deg |

### Gear Geometry (Calculated)
Final dimensions for the gear set (Pinion & Driven Wheel):

| Parameter | Symbol | Value | Unit |
| :--- | :---: | :---: | :---: |
| **Center Distance** | $a$ | 180 | mm |
| **Module (Normal)** | $m_n$ | 2.5 | mm |
| **Number of Teeth** | $z_1 / z_2$ | 18 / 115 | - |
| **Gear Width** | $b$ | 36 | mm |
| **Pressure Angle** | $\alpha_n$ | 20 | deg |

## Mechanical Analysis

### 1. Force Analysis
Forces acting on the gear mesh and transmitted to the bearings (calculated based on Torque $T_1 \approx 29.4$ Nm):
* **Tangential Force ($F_t$):** ~1209 N
* **Radial Force ($F_r$):** ~561 N
* **Axial Force ($F_a$):** ~440 N *(Due to $\beta=20^\circ$)*

### 2. Shaft & Bearing Design
* **Shaft Material:** OLC 45 (Yield Strength $\sigma_c = 360$ MPa).
* **Bearings:** Selected to withstand the combined Radial ($F_r$) and Axial ($F_a$) loads.
* **Lubrication:** Oil bath splash lubrication.

## Repository Structure

The design logic is verified through the following calculation sheets:

* **`tema de proiectare.csv`** - Initial constraints ($P=2kW, n=750rpm$).
* **`calcul geometric angrenaj.csv`** - Sizing of $z_1, z_2$ and center distance $a=180mm$.
* **`calcul arbori.csv`** - Shaft diameter sizing ($d_{prel} \approx 25-30mm$) and force calculations.
* **`durabilitatea rulmentilor.csv`** - Bearing fatigue life analysis ($L_{10}$).


### Assembly View
![2D Assembly Drawing](images/2D3D_Drawing.jpg)
*Cross-sectional view showing shaft arrangements, bearings, and gear meshing.*

### Input Shaft Drawing
![3D Model View](images/Shaft.jpg)

---
Project developed for the Mechanical Engineering curriculum.
