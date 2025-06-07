# MPPT Solar Charge Controller

This project is a **Maximum Power Point Tracking (MPPT) Solar Charge Controller** designed as part of the EEE 316 Power Electronics Laboratory course at BUET. It aims to optimize the energy harvested from photovoltaic (PV) panels by ensuring the system operates at its Maximum Power Point under varying environmental conditions.

## Overview

The controller uses the **Perturb and Observe (P\&O)** algorithm, implemented via an **Arduino Nano**, to dynamically adjust the operating point of the solar panel for maximum efficiency. A **SEPIC DC-DC converter** is employed for voltage regulation, capable of both step-up and step-down conversion depending on input conditions. The system intelligently manages charging a 12V lead-acid battery and running a load simultaneously.

## Key Features

* MPPT using P\&O algorithm
* SEPIC converter for flexible voltage management
* Real-time monitoring of voltages and currents via LCD display
* Automatic switching between solar and battery supply
* Designed for efficient energy use and safe battery operation

## Technical Highlights

* Input Voltage: 15V (from 20W solar panel)
* Output Voltage: 12V (charging)
* Switching Frequency: 50 kHz
* Efficiency: Up to 87% with MPPT vs. 61% without
* Control Unit: Arduino Nano
* MOSFET: IRFZ44N driven by IR2104 driver
* Sensors: ACS712 for current, voltage dividers for voltage sensing

## Hardware Components

* Solar panel, 20W
* 12V lead-acid battery
* SEPIC converter components (custom inductor, capacitors)
* LCD display
* Relay modules
* Arduino Nano
* ACS712 current sensor
* IRFZ44N MOSFET
* IR2104 gate driver

## Software

The firmware is written in Arduino C, implementing the MPPT algorithm and managing input/output parameters, including duty cycle adjustment and relay control.

## Implementation & Results

The project demonstrates a robust prototype that significantly improves energy transfer efficiency. It automatically adjusts to irradiance changes and maximizes solar energy usage for charging and load management.

## Links

* 🔗 [Code GitHub Repository](https://github.com/rowatulrafi)
* 🎥 [YouTube Demo](https://youtube.com)

## Future Improvements

* Integration of advanced MPPT algorithms like Incremental Conductance
* Parallel load and battery management
* Wireless monitoring capabilities
* Enhanced GUI for data visualization


