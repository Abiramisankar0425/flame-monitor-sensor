<p align="center">
  <img src="./img.png" alt="Project Banner" width="100%">
</p>

# [flame monitor sensor and safety control] 🎯

## Basic Details

### Team Name: [electrotops]

### Team Members
- Member 1: [Abirami Sankar] - [scms school of engineering and technology]
- Member 2: [Devika N S] - [scms school of engineering and technology]

### Hosted Project Link
https://drive.google.com/file/d/1RBg28Iskz1H6bXuvcXvm8cTZono6YiOS/view?usp=drivesdk

### Project Description
[ OUR PROJECT IS A FLAME MONITOR AND SAFETY SYSTEM.WHICH MONITORS THE GASTOPS,AND  REDUCE THE ACCIDENTS CAUSED BY UNNOTICED CONTINOUS FLAMES.]

### The Problem statement
[PEOPLE OFTEN FORGET ABOUT THE ON STOVE ,AND THE DISHES WILL GET RUINED AND IT CAN ALSO CUASE SERIOUS ACCIDENTS.]

### The Solution
[OUR SYSTEM ADDRESSES ALL THESE ISSUES,BY MONITORING THE FLAME CONTINOUSLY AND CUTING OFF THE FLAME IF THERE IS NOT VARAITION OF HUMAN INTERVENTON DETECTED FOR A SPECIFIC ABOUNT OF TIME(WHICH IS VARIABLE).]

---

## Technical Details

### Technologies/Components Used

**For Software:**
- Languages used: C++,ARDUINO PROGRAMMING LANGUAGE.
- Frameworks used: ARDUINO IDE
- Libraries used: servo.h
- Tools used: arduino serial monitor

**For Hardware:**
- Main components: arduino board(uno),servo motor,flame sensor,buzzer,push button,breadboard.
- Specifications:servo:0-180 degree rotation,flame sesnor:analog output (0-1023),power:5v DC
- Tools required: jumper wires,usb cable.

---

## Features

List the key features of your project:
- Feature 1: Tri-State Servo Position Control: The system automatically shifts the servo motor to three distinct positions (0^{\circ}, 90^{\circ}, and 180^{\circ}) based on the intensity of the flame detected by the analog sensor.
- Feature 2: Dual-Stage Delayed Alarm System: It features intelligent time-based monitoring that triggers the buzzer only if a High Flame persists for 5 seconds or a Low Flame persists for 8 seconds, preventing false alarms from momentary flickers
- Feature 3: Manual & Automatic Alarm Override: Users can silence the alarm using a physical push-button pulse; additionally, the system automatically stops the buzzer if the flame intensity changes to a safer level or is removed entirely
- Feature 4: Emergency Fail-Safe Shutoff: If the buzzer sounds for more than 5 seconds without user intervention, the system executes an emergency command to return the servo to the 0^{\circ} (Home) position and kill the buzzer to ensure maximum safety.

---

## Implementation

### For Software:

#### Installation
# No external package installation required
# 1. Download and install Arduino IDE from arduino.cc
# 2. Open the .ino file containing the project code

#### Run
# 1. Connect Arduino via USB
# 2. Select Board (e.g., Arduino Uno) and Port in IDE
# 3. Click 'Upload' (Control + U)
# 4. Open 'Serial Monitor' (Control + Shift + M) to view flame readings

### For Hardware:

#### Components Required
Flame Sensor Pin A0 (Analog) VCC to 5V, GND to GND
Servo Motor Pin 9 (PWM) Red to 5V, Brown/Black to GND
Buzzer Pin 8 (Digital) Positive to Pin 8, Negative to GND
Push Button Pin 7 (Digital) One side to Pin 7, Other side to GND

#### Circuit Setup
Step-by-Step Assembly
​Powering the Rails:
​Connect the Arduino 5V pin to the red (+) rail on the breadboard.
​Connect the Arduino GND pin to the blue/black (-) rail on the breadboard.
​Flame Sensor Setup:
​VCC to the 5V rail.
​GND to the GND rail.
​AO (Analog Out) to Arduino Pin A0.
​Servo Motor Setup:
​Signal (Orange) to Arduino Pin 9.
​VCC (Red) to the 5V rail.
​GND (Brown/Black) to the GND rail.
​Note: If the servo jitters, use an external 5V-6V battery pack, connecting the battery GND to the Arduino GND.
​Buzzer & Button Setup:
​Buzzer (+) to Arduino Pin 8 and (-) to GND.
​Push Button: Connect one side to Pin 7 and the other side to GND. The code uses INPUT_PULLUP, so no external resistor is needed

---

## Project Documentation

### For Software:

#### Screenshots (Add at least 3)

https://drive.google.com/file/d/1CYCUl89IZzrr62z-IsjdJ3Kmwlyig97-/view?usp=drivesdk

#### Diagrams

**System Architecture:**
https://drive.google.com/file/d/1QuDMGAX_ylTZT3bBxe6zEHVP2zEc5c11/view?usp=drivesdk

**Application Workflow:**

![Workflow](docs/workflow.png)
*Add caption explaining your workflow*

---

### For Hardware:

#### Schematic & Circuit

(https://drive.google.com/file/d/1WUQaIeFgsZIwDo8JeLRWnNAuPSuQqZSb/view?usp=drivesdk)

#### Build Photos

![Team]https://drive.google.com/file/d/1B2vJCpeRgCktg3q-UAgXoKYXqSrDg9Vn/view?usp=drivesdk

![Components] Arduino 
https://drive.google.com/file/d/1rkpRIj8Sjxyp3r7DYc19xaEcYDF07ZIZ/view?usp=drivesdk
 Push button 
https://drive.google.com/file/d/124ib-U1dUHADJ-Ky6YOxjoJIOfReCheO/view?usp=drivesdk
 Flame
https://drive.google.com/file/d/1MhH1pQMDBxadHpCkX71U3CXM6znwYjb8/view?usp=drivesdk
 Buzzer 
https://drive.google.com/file/d/1MgGNw3vlFsgK6eyeXlz2bccr_taN3pXY/view?usp=drivesdk
 Servo 
https://drive.google.com/file/d/1xh5WcCGF-tDpsRuRybw7CV8UDtwSlm42/view?usp=drivesdk

![Build](Add photos of build process here)
*Explain the build steps*

![Final](https://drive.google.com/drive/folders/1AbOSknTNM2mketG4gX9uV-hy6HdCVN3h)

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

#### Assembly Instructions

**Step 1: Prepare Components**
1. Gather all components listed in the component list
2. Check component specification and its working.

**Step 2: Build the Power Supply**
1. Connect the power rails on the breadboard
2. Connect Arduino 5V to breadboard positive rail
3. Connect Arduino GND to breadboard negative rail
![Step 2](images/assembly-step2.jpg)
*Caption: Power connections completed*

**Step 3: Add Components**
1. Place LEDs on breadboard
2. Connect resistors in series with LEDs
3. Connect LED cathodes to GND
4. Connect LED anodes to Arduino digital pins (2-6)
![Step 3](images/assembly-step3.jpg)
*Caption: LED circuit assembled*

**Step 4: [Continue for all steps...]**

**Final Assembly:**
(https://drive.google.com/file/d/1RBg28Iskz1H6bXuvcXvm8cTZono6YiOS/view?usp=drivesdk)



## Project Demo

### Video
(https://drive.google.com/file/d/1RBg28Iskz1H6bXuvcXvm8cTZono6YiOS/view?usp=drivesdk)

*Explain what the video demonstrates - key features, user flow, technical highlights*

### Additional Demos
[Add any extra demo materials/links - Live site, APK download, online demo, etc.]

---

## AI Tools Used (Optional - For Transparency Bonus)

If you used AI tools during development, document them here for transparency:

**Tool Used:** chatgpt ,gemini

**Purpose:**
- for getting code ready.

**Key Prompts Used:**
gnerate the code to assign the servo motions wrt to flame intensity
**Percentage of AI-generated code:** 90 percetnage

**Human Contributions:**
-prompting,the project idea,project specifications,testing of product.



## Team Contributions

abhirami did with hardware,wiring.
devika did the simulation,prompting.
both equally contriuted to testing phase


## License

This project is licensed under the [LICENSE_NAME] License - see the [LICENSE](LICENSE) file for details.

**Common License Options:**
- MIT License (Permissive, widely used)
- Apache 2.0 (Permissive with patent grant)
- GPL v3 (Copyleft, requires derivative works to be open source)

---

Made with ❤️ at TinkerHub
