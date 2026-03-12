# Mixed-Signal Precision Instrumentation System

## Overview
A 4-stage analog conditioning chain engineered for high-precision sensor interfacing.The system utilizes **AD8030** rail-to-rail op-amps to provide robust signal processing from differential input to rectified output.

## System Architecture
* **Instrumentation Amplifier:** 3-op-amp topology with **8 V/V gain** and **108 dB CMRR** for superior noise rejection.
* **Band-Pass Filter:** Sallen-Key topology tuned to **$f_0$ = 14.1 kHz** ($Q = 1.41$).
* **Programmable Gain Amplifier (PGA):** 4 digital steps (**5, 7, 9, 11 dB**) via parallel resistor switching.
* **Precision Rectifier:** Full-wave AC-DC converter with **2 V/V gain** for ADC compatibility.

## Performance Summary
| Metric | Specification | Simulated (LTSpice) | Measured (Hardware) |
| :--- | :--- | :--- | :--- |
| **IA Gain** | 8 V/V | 7.93 V/V  | 9 V/V  |
| **Filter $f_0$** | 14.1 kHz | 14.1 kHz | 14.01 kHz |
| **THD** | < 1% | 0.11% | OK |
| **PGA Max Gain**| 11 dB | 10.99 dB | 10.96 dB |

## Technical Skills Demonstrated
* **Simulation:** DC op, AC sweep, Transient, and THD analysis in LTSpice/PSpice.
* **Hardware:** Breadboard prototyping, digital oscilloscopes, and logic analyzers.
* **Design:** High-precision analog signal conditioning and hardware-software co-design.
