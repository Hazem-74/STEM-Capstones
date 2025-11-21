# Automonitor Trough System (Concentrated Solar Power)  
Grade 12 Capstone Project | Sharkia STEM School | 2021–2022

SDGs: SDG 7 (Affordable & Clean Energy), SDG 9 (Industry & Innovation), SDG 13 (Climate Action)

## Problem Statement
Concentrated Solar Power (CSP) plants consume significant electricity to run feedwater pumps continuously—even when thermal oil is sufficiently hot—reducing net efficiency.

## Scientific Principles

### Thermal Regulation and Control
The system uses an NTC temperature sensor to activate the feedwater pump only when thermal oil temperature ≥ 110°C and deactivate it at ≤ 90°C. Energy savings follow:  
$E = P \cdot t = (I \cdot V) \cdot t$

### Optical Geometry
Parabolic trough dimensions were derived from concentration ratio equations:  
- Aperture width: 65 cm  
- Focal distance: 16.25 cm  
- Rim angle: 90°  
- Maximum concentration ratio: **C = 68.3**

### IoT Integration
- **Arduino-based control** with Wi-Fi module (RemoteXY) for real-time temperature monitoring
- **Sun-tracking system** using LDRs and stepper motor to maintain optimal focal alignment

## Results
| Metric                | Without Control | With Control | Improvement |
|-----------------------|------------------|---------------|-------------|
| Pump runtime          | 92 s             | 78 s          | ↓ 15.2%     |
| Electrical energy     | 7.728 J          | 6.552 J       | ↓ 15.21%    |
| Steam output          | 40 ml            | 35 ml         | Slight trade-off |

In a 50 MW plant (e.g., Andasol 3), this saves **145.56 kW** of parasitic load.

## Physics and Engineering Concepts
- Stefan-Boltzmann law (radiative heat transfer)
- Ohm’s law and electrical power ($P = IV$)
- Parabolic reflector optics and focal geometry
- Feedback control systems in IoT

## Real-World Impact
This system increases net CSP efficiency and supports Egypt’s target of **42% renewable energy by 2035**.

## Acknowledgments
We thank Mr. Ahmed Ashour, Mrs. Mohammed El-Zeftawy, Mr. Hany Boules, and Eng. Ahmed Farok for technical support.
