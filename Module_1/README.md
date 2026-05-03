# Module 1 - Introduction to Verilog RTL Design and Synthesis

## Subtopic: Introduction to Open-Source Simulator (Iverilog)

---

## Objective

To understand the basics of Verilog design, simulation, and testbench.

---

## Theory

### 🔹 Simulator

* RTL design is verified by simulating the design.
* Simulator checks whether the design meets the required specifications.
* Iverilog is the simulator used in this course.

### 🔹 Design

* Design refers to the actual Verilog code.
* It implements the required functionality of the system.

### 🔹 Testbench

* Testbench is used to apply input stimulus (test vectors) to the design.
* It helps verify the correctness of the design.

### 🔹 How Simulator Works

* Simulator monitors changes in input signals.
* When input changes, output is evaluated.
* If there is no change in input, output remains unchanged.

---

## Simulation Flow

* Design and Testbench are given as input to the simulator.
* Simulator generates output in the form of waveform (VCD file).
* Output is visualized using waveform viewer (GTKWave).

---

## Screenshots

### 1. PPT / Theory Reference

(Add screenshot of the PPT slide here)

### 2. Simulation Flow Diagram

(Add screenshot of simulation flow if shown in video)

---

## Conclusion

Understood the basic concepts of simulator, design, and testbench along with the working of Iverilog simulation flow.

---

---

## Subtopic 2: Labs using iverilog and gtkwave

---

We have to add a github repository which will contain all the files and tools we will be needing.
We used this command to add the repository:
```bash
git clone https://github.com/vsdip/vsd-rtl.git

```
![Output](./screenshots/output2.png)

Now in this repo we can see the sky130RTLDesignAndSynthesisWorkshop directory, which will have lib directory containing sky130 standard cell library and also the my_lib directory containg the verilog models and finally the verilog_files directory containing all the verilog files which we will be using during our labs.

---


