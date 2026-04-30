# 🚀 RV12 Pipeline CPU (Verilog)

A modular **6-stage pipelined RISC-V CPU** designed in Verilog, inspired by RV12 architecture.
This project demonstrates practical CPU design concepts including instruction flow, pipeline stages, and simulation.

---

## 🔷 🧩 Pipeline Architecture

The processor follows a **6-stage pipeline**:

```
IF → PD → ID → EX → MEM → WB
```

* **IF (Instruction Fetch)** – Fetch instruction from memory
* **PD (Pre-Decode)** – Instruction alignment / preprocessing
* **ID (Decode)** – Register read + instruction decode
* **EX (Execute)** – ALU operations
* **MEM (Memory)** – Data memory access
* **WB (Write Back)** – Write result to register file

---

## 🔷 ⚙️ Features

* ✅ Modular design (each stage in separate module)
* ✅ Clean pipeline data flow
* ✅ Register file with write-back support
* ✅ Simple ALU (ADD operation implemented)
* ✅ Fully testbench verified
* ✅ Vivado simulation compatible

---

## 🔷 📂 Project Structure

```
📁 RV12-Pipeline-CPU
 ┣ 📄 IF_stage.v
 ┣ 📄 PD_stage.v
 ┣ 📄 ID_stage.v
 ┣ 📄 EX_stage.v
 ┣ 📄 MEM_stage.v
 ┣ 📄 WB_stage.v
 ┣ 📄 pipeline_top.v
 ┗ 📄 tb_pipeline.v
```

---

## 🔷 ▶️ Simulation (Vivado)

### Steps:

1. Open Vivado → Create Project
2. Add all `.v` files
3. Set `tb_pipeline` as Top Module
4. Run **Behavioral Simulation**

---

## 🔷 📊 Sample Output

```
Time=0   PC=00000000 EX_RESULT=00000000
Time=10  PC=00000004 EX_RESULT=0000001E
Time=20  PC=00000008 EX_RESULT=00000032
```

✔ Shows multiple instructions executing in pipeline
✔ Confirms correct ALU operations

---

## 🔷 ⚠️ Current Limitations

* ❌ No hazard detection
* ❌ No forwarding logic
* ❌ No branch handling
* ❌ Supports only basic operations

---

## 🔷 🚀 Future Improvements

* 🔄 Hazard Detection Unit
* 🔄 Forwarding Unit
* 🔄 Branch Prediction
* 🔄 Full RISC-V instruction support
* 🔄 Memory interface (AHB/AXI)

---

## 🔷 🎯 Learning Outcome

* Practical understanding of CPU pipeline
* Hands-on Verilog design
* Simulation & debugging in Vivado
* Foundation for VLSI / Processor design roles

---

## 🔷 👨‍💻 Author

**Kubendran S**
📍 VLSI & Embedded Systems Enthusiast

---

## ⭐ If you like this project

Give a ⭐ on GitHub and share with others 🚀
