# Module 1 - Introduction to Verilog RTL Design and Synthesis

## Subtopic 1: Introduction to Open-Source Simulator (Iverilog)

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
![how sim works](./screenshots/1.1.png)

---

## Simulation Flow

* Design and Testbench are given as input to the simulator.
* Simulator generates output in the form of waveform (VCD file).
* Output is visualized using waveform viewer (GTKWave).
![sim flow](./screenshots/1.2.png)

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
![Output](./screenshots/2.1.png)

Now in this repo we can see the sky130RTLDesignAndSynthesisWorkshop directory, which will have lib directory containing sky130 standard cell library and also the my_lib directory containg the verilog models and finally the verilog_files directory containing all the verilog files which we will be using during our labs.

---

Now we will work in verilog_files directory. In this directory we can see verilog designs and their corresponding TestBench files(startng with tb_).
command to launch a MUX file using iverilog:
```bash
iverilog good_mux.v tb_good_mux.v
./a.out
gtkave tb_good_mux.vcd
```

NOTE: if any tool is not installed, intall it using
```bash
sudo apt install _____
```
![sim flow](./screenshots/2.2.png)

Now the GTKWave window will open. Just drag and drop the inputs and Zoom fit to see the output waveform for the MUX.
![sim flow](./screenshots/2.3.png)

---

Now we will look at the file structure of the verilog files. run the command:
```bash
gvim good_mux.v -o tb_good_mux.v
```
![sim flow](./screenshots/2.4.png)
Here we can see the differences between Design and TestBench files and also change the simulation time in the TestBench file.
Hence this file serves as the Simualtion generator.

---
