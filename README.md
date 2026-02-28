# Pressure Measurement System Design using MPX5500 Sensor

## Project Overview
This project focuses on designing and simulating a high-precision pressure measurement system. The system converts physical pressure (0-500kPa) into an analog voltage (0-9V) and processes it via a 10-bit ADC for digital monitoring.

## Key Features
- **Pressure Range:** 0 to 500 kPa.
- **Output Voltage:** Linear mapping from 0V to 9V.
- **Accuracy:** Error margin maintained within ±5% through precision signal conditioning.
- **ADC Integration:** Signal scaled for 10-bit ADC processing on ATmega328P (Arduino).

## Technical Implementation
### 1. Signal Conditioning
- Utilized **LT1014CN Op-Amps** for offset nulling and gain amplification.
- Designed a low-pass filter to eliminate sensor noise and interference.
- Performed rigorous calculations for component selection (1% tolerance resistors) to ensure stability.

### 2. Simulation & Verification
- **Tools:** NI Multisim, Proteus.
- Simulated the full signal chain: Sensor -> Amplification -> Filtering -> Voltage Division.
- Verified Voltage Transfer Characteristics (VTC) against theoretical datasheets.

### 3. Data Processing
- Implemented a voltage divider (1:2 ratio) to protect the MCU's 5V input.
- Calculated resolution and ADC steps to ensure 1kPa measurement precision.

## Tools & Technologies
- **Hardware Simulation:** NI Multisim, Proteus.
- **Embedded:** ATmega328P (Arduino), C++.
- **Documentation:** Microsoft Office, Datasheet Analysis.

## Results
The simulation results achieved a near 1% error rate, successfully mapping the 0-500kPa range to a digital-friendly format, ready for real-world hardware implementation.
[🎥 Xem video demo hệ thống tại đây]([link-google-drive-cua-ban](https://drive.google.com/file/d/1bqTe8eYmdHC43heR7EktlxG5tiRI9o3g/view?usp=drive_link))
