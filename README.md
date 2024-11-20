# Embedded Systems Lab 7: CMSIS-DSP Programming

This repository contains the solution to **Lab 7: CMSIS-DSP Programming**. The project demonstrates the implementation of **DSP algorithms** on an **STM32 microcontroller**, processing sensor data and validating results using known test signals and real-world data.

---

## Problem Statement

The objective of this lab is to design a DSP program using **STM32CubeIDE** to process sensor data from the **STM32 IoT Node development board**. The lab requires the implementation of DSP algorithms, such as a **low-pass filter (FIR)** or **FFT**, and validation of the program with both test signals and actual sensor data. Additionally, there is an optional challenge to extend functionality using **CMSIS-RTOS2**.

### Requirements

1. **DSP Algorithm Implementation (DONE)**:
   - Process sensor data (e.g., from 3D accelerometers or gyroscopes).
   - Implement a DSP algorithm such as a **low-pass filter** (e.g., FIR) or **FFT**.
   - Test the program with a known signal to validate correctness before testing real data.

2. **Optional Challenge: Multi-Tasking with CMSIS-RTOS2** (*+10 points*) (DONE):
   - Design three tasks scheduled by **CMSIS-RTOS2**:
     1. **Sensor Data Acquisition**: The highest-priority task, triggered by a timer, periodically reads sensor data.
     2. **Data Processing**: Processes the acquired data using a digital filter (e.g., low-pass filter).
     3. **Data Transmission**: Sends both raw and processed data via **Wi-Fi** or **BLE** to a PC or Raspberry Pi for visualization and validation.
