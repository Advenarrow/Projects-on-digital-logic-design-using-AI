# Projects on Digital Logic Design using AI

This repository contains digital logic design implementations where **Artificial Intelligence (AI)** was utilized to assist in the generation, optimization, or verification of Hardware Description Language (HDL) code. The project focuses on bridging the gap between traditional logic design and AI-assisted engineering.

## 📁 Repository Structure

The repository consists of two primary modules implemented in Jupyter Notebooks (`.ipynb`), integrating Verilog/VHDL logic with simulation and visualization tools.

* **`4-to-1-MUX.ipynb`**: Implementation and verification of a 4-to-1 Multiplexer.
* **`UART-Baud-Generator.ipynb`**: A precise clock divider circuit designed to generate standard baud rates for UART communication.

---

## 🚀 Projects Overview

### 1. 4-to-1 Multiplexer (MUX)
A fundamental combinational logic circuit that selects one of four binary inputs and forwards it to a single output line based on two select signals.
* **Logic Expression**: $Y = S_1'S_0'I_0 + S_1'S_0I_1 + S_1S_0'I_2 + S_1S_0I_3$
* **AI Integration**: Used for generating optimized behavioral Verilog code and creating comprehensive testbench stimulus.

### 2. UART Baud Rate Generator
A sequential logic circuit that divides a high-frequency system clock (e.g., 50MHz or 100MHz) down to a specific pulse frequency required for UART transmission (e.g., 9600, 115200 bps).
* **Key Feature**: Configurable divisors to support multiple standard baud rates.
* **AI Integration**: Used to calculate precise divisor constants and verify timing constraints within the Verilog module.

---

## 📈 Simulation and Waveforms

The verification of these designs is performed using **Icarus Verilog** for simulation and **GTKWave** for waveform visualization.

### Viewing the Output
To view the digital timing diagrams:
1.  Run the cells within the `.ipynb` files to generate the `.vcd` (Value Change Dump) files.
2.  Open the generated file using GTKWave:
    ```bash
    gtkwave simulation_output.vcd
    ```

#### Expected GTKWave Outputs:
* **MUX**: You will observe the output `Y` changing strictly according to the select lines `S1` and `S0`.
* **UART**: You will see the `baud_tick` signal pulsing at the exact intervals calculated for the target bit rate.



---

## 🛠️ Tools & Technologies
* **Languages**: Verilog / SystemVerilog
* **Environment**: Jupyter Notebook
* **Simulator**: Icarus Verilog
* **Waveform Viewer**: GTKWave
* **AI Tools**: Used for code scaffolding and logic optimization.

---

## ⚙️ How to Use
1.  **Clone the Repository**:
    ```bash
    git clone https://github.com/YourUsername/Projects-on-digital-logic-design-using-AI.git
    ```
2.  **Install Dependencies**: Ensure you have `iverilog` and `gtkwave` installed on your system.
3.  **Run Notebooks**: Open the `.ipynb` files in VS Code or Jupyter Lab and run all cells to execute the simulations.

---

## 🤝 Contributing
Feel free to fork this repository and submit pull requests if you have AI-assisted optimizations or new digital logic modules to add!
