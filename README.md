# Dynamic Modelling of a Separately-Excited DC Electric Motor

## 📌 Project Overview

This project implements the dynamic model of a separately-excited **DC motor** using **MATLAB/Simulink**. The simulation analyzes the motor's electrical and mechanical behavior under different conditions, providing insights into speed and current characteristics.

## 🎯 Objectives

- Develop and simulate the **mathematical model** of a separately-excited DC motor.
- Analyze motor performance under **no-load** and **loaded conditions**.
- Visualize motor behavior through **speed and current waveforms**.

## 🏷️ Methodology

The project is based on fundamental mathematical equations governing DC motor operation. The **Simulink model** includes:

- **Electrical Equation**
- **Mechanical Motion Equation**
- **Electromagnetic Torque Equation**

## ⚙️ Simulink Implementation

The model was built using:

- **Integrator Blocks** (for speed and current computation)
- **Gain Blocks** (for resistances, inductances, constants, etc.)
- **Sum Blocks** (for algebraic operations)
- **Constant Blocks** (for input voltage and load torque)
- **Scope Blocks** (for visualization of results)

## 📊 Simulation Parameters

| Parameter                   | Value            |
| --------------------------- | ---------------- |
| Armature Resistance \(R_a\) | 0.5 Ω            |
| Armature Inductance \(L_a\) | 0.003 H          |
| Back EMF Constant \(K_b\)   | 0.8 V/rad/sec    |
| Load Inertia \(J\)          | 0.0167 Kg.m²     |
| Damping Coefficient \(B\)   | 0.01 N.m/rad/sec |
| Supply Voltage \(V\_{in}\)  | 220 V            |

## 🏁 Simulation Conditions

The model was simulated under two conditions:

1. **No Load Condition:** The motor was supplied with a constant DC voltage of 220 V while the load torque \(T_L\) was set to zero.
2. **Loaded Condition:** A load torque of **100 N.m** was applied to observe its impact on speed and current.

### 🔄 Solver Configuration

To ensure numerical stability and accuracy, the solver settings in Simulink were configured as follows:

- **Solver:** ode23tb (suitable for stiff electrical systems)
- **Simulation Time:** 0.1 seconds

## 🖥️ Results

The following results were obtained from the simulation:

- **Fig. 1:** Simulink Model of the DC Motor
- **Fig. 2:** Motor Speed at No Load Condition
- **Fig. 3:** Motor Speed with Applied Load Torque
- **Fig. 4:** Armature Current at No Load Condition
- **Fig. 5:** Armature Current with Applied Load Torque
- **Fig. 6:** Combined Simulation Results

## 📌 Conclusion

This project successfully models and simulates a separately-excited DC motor's dynamic behavior under different operating conditions. MATLAB/Simulink proved to be an effective tool for analyzing motor performance, demonstrating variations in speed and current due to changes in load torque.

## 📂 Repository Structure

```
🗂 Dynamic Model of a DC Electric Motor
 ├── 📚 DYNAMIC MODELLING OF DC ELECTRIC MOTOR.pdf  # Project report
 ├── 🔬 DYNAMIC MODELLING OF DC ELECTRIC MOTOR.slx   # Simulink model
 ├── 📝 README.md       # Project documentation (this file)
```

## 🚀 How to Run the Simulation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Michael-ola/Dynamic-Model-of-a-DC-Electric-Motor.git
   ```
2. **Open MATLAB and navigate to the project folder**
3. **Run the Simulink model:** Open the `.slx` file and click **Run**
4. **View results:** Open the Scope blocks to analyze the waveforms
