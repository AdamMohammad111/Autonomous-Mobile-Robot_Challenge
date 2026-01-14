# Autonomous Mobile Robot Challenge (PIC16F877A) – PSUT Embedded Systems

This repository contains our **Autonomous Mobile Robot Challenge** project for the **Embedded Systems Class** at **Princess Sumaya University for Technology (PSUT)**.

## Project Overview
The robot completes the challenge track using the following behavior flow:
1. **Line Following** using IR line sensors  
2. **Tunnel Detection** using an LDR (buzzer active while inside tunnel)  
3. **Left Wall Following** after tunnel using **two ultrasonic sensors**  
4. **Re-catch Line** after wall-following and enable parking trigger  
5. **Parking Stage**: slow approach + beep pattern + final stop + servo flag

## Hardware (Summary)
- **MCU:** PIC16F877A (mikroC PRO for PIC, 8 MHz)
- **Line Sensors:** IR sensors (RB4, RB5)
- **Tunnel Sensor:** LDR on ADC (RA0)
- **Ultrasonic Sensors:**
  - Front: TRIG RD0, ECHO RC3 (or RD1 depending on wiring)
  - Left:  TRIG RD4, ECHO RD5
- **Obstacle IR Sensors:** RC5 (Left), RD3 (Right)
- **Motors:** Dual DC motors via driver (PWM on CCP1/CCP2)
- **Servo:** RA2 (flag mechanism)
- **Buzzer:** RB7
- **LED:** RB6

## Repository Contents
- `Report/` → Final report (PDF/DOCX)
- `Poster/` → Poster file (PDF + optional editable format)
- `Code/` → Full project folder (ZIP) + source + compiled HEX
- `Media/Pics/` → Photos of the robot and wiring
- `youtube.txt` → YouTube demo link
- `GitHub.txt` / `GitHib.txt` → Repository URL for submission

## How to Run (mikroC)
1. Open the project in **mikroC PRO for PIC**
2. Select device: **PIC16F877A**
3. Set clock: **8 MHz**
4. Build the project to generate the **.hex**
5. Upload the hex to the PIC using your programmer, or simulate in Proteus if applicable

## Video Demo
See `youtube.txt` for the demo URL.

## Authors
- (Add your names here)
