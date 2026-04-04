<p align="center">
  <img src="./img.png" alt="Project Banner" width="100%">
</p>

# flame monitor sensor and safety control 🎯

## Basic Details

### Team Name: electrotops

### Team Members
- Member 1: [Abirami Sankar] - [scms school of engineering and technology]
- Member 2: [  Devika N S  ] - [scms school of engineering and technology]

### Hosted Project Link
https://drive.google.com/file/d/1RBg28Iskz1H6bXuvcXvm8cTZono6YiOS/view?usp=drivesdk

### Project Description
 OUR PROJECT IS "THE FLAME MONITOR AND SAFETY SYSTEM". WHICH MONITORS THE GASTOPS AND  REDUCE  ACCIDENTS CAUSED BY UNNOTICED CONTINUOUS FLAMES.

### The Problem statement
FORGETTING FOOD ON THE STOVE CAN RUIN THE MEALS, CAUSE COOKING GAS WASTAGE AND POSE SERIOUS SAFETY RISKS.

### The Solution
OUR SYSTEM ADDRESSES ALL THESE ISSUES BY MONITORING THE FLAME CONTINUOUSLY AND CUTTING OFF THE FLAME IF THERE IS NO HUMAN INTERVENTION DETECTED, FOR A PARTICULAR AMOUNT OF TIME (WHICH IS VARIABLE).

---

## Technical Details

### Technologies/Components Used

**For Software:**
- Languages used: C++,ARDUINO PROGRAMMING LANGUAGE.
- Frameworks used: ARDUINO IDE
- Libraries used: servo.h
- Tools used: Arduino serial monitor

**For Hardware:**
- Main components: Arduino board(uno), servo motor,flame sensor,buzzer,push button, breadboard.
- Specifications:servo:0-180 degree rotation, flame sensor: analog output (0-1023), power: 5V DC
- Tools required: jumper wires, USB cable.

---

## Features

List the key features of your project:
- Feature 1: Tri-State Servo Position Control (Stove Knob Indicator)
The system automatically positions the servo motor at three predefined angles to represent flame conditions:

0° → No flame
−90° → High flame
−180° → Low flame

These positions are determined based on the intensity of the flame detected by the analog sensor.

In real gas stoves, flame intensity changes gradually as the knob is rotated. However, due to limited components, the system assumes an instantaneous response and does not account for the time delay between knob rotation and flame stabilisation.
- Feature 2: Dual-Stage Delayed Alarm System: It features intelligent time-based monitoring that triggers the buzzer only if a High Flame persists for 5 seconds or a Low Flame persists for 8 seconds, preventing false alarms from momentary flickers.(The time set is variable here)
- Feature 3: Manual & Automatic Alarm Override: Users can silence the alarm using a physical push-button pulse; additionally, the system automatically stops the buzzer if the flame intensity changes to a safer level or is removed entirely.
- Feature 4: Emergency Fail-Safe Shutoff: If the buzzer sounds for more than 5 seconds without user intervention, the system executes an emergency command to return the servo to the 0^{\circ} (Home) position and kill the buzzer to ensure maximum safety.

---

## Implementation

### For Software:

#### Installation
 No external package installation required
 1. Download and install Arduino IDE from arduino.cc
 2. Paste the project code into the Code Editor (Sketch Area) and run the code.

#### Run
 1. Connect Arduino via USB
 2. Select Board (e.g., Arduino Uno) and Port in IDE
 3. Click 'Upload' (Control + U)
 4. Open 'Serial Monitor' (Control + Shift + M) to view flame readings

### For Hardware:

#### Components Required
 1. Flame Sensor Pin A0 (Analog) VCC to 5V.
 2. GND to GND.
 3. Servo Motor Pin 9 (PWM) Red to 5V, Brown/Black to GND.
 4. Buzzer Pin 8 (Digital) Positive to Pin 8, Negative to GND.
 5. Push Button Pin 7 (Digital) One side to Pin 7, Other side to GND.

---

## Circuit setup

### Step-by-Step Assembly
          
#### powering the rails
1. Connect the Arduino 5V pin to the red (+) rail on the breadboard.
2. ​Connect the Arduino GND pin to the blue/black (-) rail on the breadboard.


#### ​Flame Sensor Setup:
1. ​VCC to the 5V rail.
2. ​GND to the GND rail.
3. AO (Analog Out) to Arduino Pin A0.
  

#### ​Servo motor setup:
1. Signal (Orange) to Arduino Pin 9.
2. VCC (Red) to the 5V rail.
3. GND (Brown/Black) to the GND rail.

​Note: If the servo jitters, use an external 5V-6V battery pack and connect the battery GND to the Arduino GND.

#### ​Buzzer & Button Setup:
​1. Buzzer (+) to Arduino Pin 8 and (-) to GND.
#### ​Push Button:
1. Connect one side to Pin 7 and the other side to GND. The code uses INPUT_PULLUP, so no external resistor is needed

**Final Assembly:**

<img width="1400" height="1000" alt="image" src="https://github.com/user-attachments/assets/ec2faaab-f724-4c68-bee9-500f2b6c557d" />

---

## Project Documentation

### For Software:

#### Screenshots 
**ARDUINO IDE: code running and output on serial monitor**
https://drive.google.com/file/d/1CYCUl89IZzrr62z-IsjdJ3Kmwlyig97-/view?usp=drivesdk

#### Diagrams

**System Architecture:**
<img width="1041" height="919" alt="system arch" src="https://github.com/user-attachments/assets/ab611547-f067-4f2f-b04e-e583728db525" />




---

### For Hardware:

#### Schematic & Circuit

(https://drive.google.com/file/d/1WUQaIeFgsZIwDo8JeLRWnNAuPSuQqZSb/view?usp=drivesdk)

### Team
![team png](https://github.com/user-attachments/assets/9ab316fe-ef65-4301-87d8-766929d85ca7)

#### components Photo

#### Components
1. Arduino UNO
https://drive.google.com/file/d/1rkpRIj8Sjxyp3r7DYc19xaEcYDF07ZIZ/view?usp=drivesdk
2. Push button 
https://drive.google.com/file/d/124ib-U1dUHADJ-Ky6YOxjoJIOfReCheO/view?usp=drivesdk
3.  Flame sensor
https://drive.google.com/file/d/1pS8cAkXfdaMsLc2w9xU1zE7mrl8lVjI_/view?usp=sharing
4. Buzzer 
https://drive.google.com/file/d/1MgGNw3vlFsgK6eyeXlz2bccr_taN3pXY/view?usp=drivesdk
5.  Servo motor
https://drive.google.com/file/d/1xh5WcCGF-tDpsRuRybw7CV8UDtwSlm42/view?usp=drivesdk


---


### For Hardware Projects:

#### Bill of Materials (BOM)

| Component                      | Quantity | Specifications          | Price    | Link/Source |
|--------------------------------|----------|-------------------------|----------|-------------|
| Arduino Uno                    | 1        | ATmega328P, 16MHz       | ₹450     | [Link]      |
|Flame Sensor Module(IR based)   | 1        |760–1100 nm  IR spectrum |₹90 – ₹150| [Link]
|Piezo Buzzer (Active)           | 1        |5V DC active buzzer      | ₹40      | [Link]      |
| Servo Motor                    | 1        |5 V, 180° rotation       | ₹180     | [Link]      |
| Breadboard                     | 1        | 830 points              | ₹100     | [Link]      |
| Jumper Wires                   | 20       | Male-to-Male            | ₹50      | [Link]      |
|push button switch              | 1        |manual control           | ₹15      | [Link]      |


**Total Estimated Cost:** ≈ ₹1,015 – ₹1,685 



## Project Demo

### Video
(https://drive.google.com/file/d/1RBg28Iskz1H6bXuvcXvm8cTZono6YiOS/view?usp=drivesdk)


## AI Tools Used (Optional - For Transparency Bonus)

**Tools Used:** chatgpt ,gemini.

**Purpose:**
- for getting the code ready.

**Key Prompts Used:**
Generate the code to assign the servo motions wrt to the flame intensity.
**Percentage of AI-generated code:** 90%.

**Human Contributions:**
-the project idea,prompting, project assembly, debugging the errors and testing of product.



## Team Contributions

1. abhirami did with hardware and wiring.
2. devika did the simulation, prompting.
3. Both equally contributed to the debugging and testing phase.


---

Made with ❤️ at TinkerHub
