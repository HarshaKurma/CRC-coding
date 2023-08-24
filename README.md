# Verilog code of 16 bit serial CRC coding

This repository contains a Verilog testbench for the `CRC_serial16` module, designed for CRC (Cyclic Redundancy Check) calculations.

## Overview

The `CRC_serial16` module is a Verilog implementation of a CRC encoder. This testbench is designed to verify the functionality of the module by applying different test cases and validating the CRC calculations.

## Module Parameters

- `LENGTH`: Set to 368 bits (you can adjust this as needed).

## How to Use

1. **Simulation Setup**: To run the simulation, make sure you have a Verilog simulator (e.g., ModelSim) installed.

2. **Test Messages**: The `msg` variable contains the test message that will be processed by the CRC encoder. You can modify the message by changing the `msg` assignment.

3. **Enabling the CRC Encoder**: The testbench initializes the CRC encoder by setting `iEn` to 1 and `iRST` to 0 after a brief reset period.

4. **Message Encoding**: The testbench processes the message bit by bit, sending it to the CRC encoder using the `iMSG` input.

5. **Results**: The simulation displays the original message, the CRC calculation, and a result message indicating whether the CRC calculation is successful or not.

6. **Simulation Termination**: The simulation stops when it's complete, and the result is displayed.


