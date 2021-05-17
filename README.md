# FPGA Project Repository

## Purpose
The purpose of this project is for an engineer to learn some FPGA concepts from the ground up. It will start relatively slowly and progress into a small project similar to a small project that one might find in an industry setting. Everything that gets written will be replicated with both Verilog and VHDL for educational purposes, with Verilog and SystemVerilog being the main focus due to its popularity in various industries. VHDL is still used by some companies but in the US, Verilog is currently more widely used.

### 1. Create a PRN generator/counter | Difficulty -- beginner.

The objective of this task is to create 1 module that starts a PRN counter for output. This task will cover concepts such as pulse-starts for tasks, initial conditions/seeds, and FSMs.

* Create a module with the following inputs/outputs
  * Clock **input**
  * Reset **input** (active low or high, doesn't matter)
  * 32-bit seed **input**
  * 32-bit count **input**
  * 1-bit start pulse **input**
  * 32-bit PRN **output**
* Use an FSM for the logic
  * Start pulse kicks off the output PRN sequence
  * Output count amount of words before stopping and returning to IDLE state
  * Seed will be the first number to start the PRN sequence with
  * Use any 32-bit PRN algorithm, can look up online
  * Use **synchronous** reset for logic
* Write a simple testbench to test the functionality of design
  * Can simulate online with various web-simulators
  * Can get Vivado Webpack which is FREE and comes with ModelSim
