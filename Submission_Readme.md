# ⚡ Energy-Adaptive Sensor Data Processing on Microwatt  
_A Reconfigurable SoC for Low-Power Edge Intelligence_  

---

## 📄 Problem Statement
The rapid growth of **edge computing** has created a demand for systems that can efficiently process **heterogeneous sensor data** while maintaining strict **energy** and **latency** constraints.  

Applications such as:  
- 🩺 **Continuous ECG monitoring**  
- ✋ **Gesture recognition in wearables**  
- 🌍 **Environmental sensing in IoT devices**  

all require a **balance** between:  
- 🔋 **Low-power streaming operations**  
- ⚡ **High-performance compute bursts**

---

## 🚧 Current Limitations
Existing solutions fall into two extremes:  
1. 🛠️ **Fixed-function accelerators** → Energy-efficient but rigid ❌  
2. 🖥️ **General-purpose CPUs** → Flexible but inefficient ❌  

This gap prevents **scalable, energy-adaptive edge intelligence**, especially in **medical & wearable domains** where:  
- Continuous operation is critical  
- Battery resources are limited  

---

## 💡 Proposed Solution
We propose an **Energy-Adaptive Sensor Data Processor (EASDP)** tightly coupled with the **open-source Microwatt CPU core**.  

### 🔀 Dual Operating Modes
1. **Streaming Mode** → Continuous, low-power operations  
   - FIR/IIR filtering  
   - Feature extraction (e.g., R-peak detection for ECG)  

2. **Burst Mode** → Compute-intensive tasks  
   - Gesture recognition  
   - Keyword spotting  
   - Compact **MAC (Multiply-Accumulate) array**  

---

## 🧩 Key Components
- ⚙️ **Reconfigurable Sensor Processing Unit (SPU)** → Handles both streaming & burst workloads  
- 🕹️ **Lightweight Control & Policy Unit** → Dynamically switches modes based on:  
  - Workload activity  
  - Latency requirements  
  - Energy constraints  

Result 👉 Optimal **performance per watt** ✅  

---

## 🏗️ Implementation Details
- 🖧 **Architecture** → Modular & fully digital  
- 🧱 **Technology** → SkyWater 130nm (**SKY130**)  
- 🔓 **Open-Source Flows** → Yosys, Verilator, OpenLane  
- 📦 **Integration** → Fits within **ChipFoundry OpenFrame** user project area  
- ✅ **Tapeout-Ready** → Filters, MAC arrays & FSM control ensure feasibility  

---

## 🌟 Impact
✨ First **open-source Microwatt-based SoC** with **runtime energy-adaptive sensor processing**.  
✨ Bridges the gap between **CPU flexibility** and **accelerator efficiency**.  
✨ Fabrication-ready design with novelty, adaptability, and real-world impact.  

---

## 👨‍💻 Contributors
- 📝 Sankararayanan V
- 📝 chezhiyan M
- 📝 Ebinesh K

