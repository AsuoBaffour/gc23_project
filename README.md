# gc23_project
Fire Alarm System


Table of Contents

Introduction
Features
Project Structure
Getting Started
Usage
Web Interface
Contact
Technologies Used

Introduction
This project is a comprehensive fire alarm system that utilizes a Raspberry Pi's GPIO (General-Purpose Input/Output) pins in conjunction with a flame sensor to detect and respond to potential fire hazards. When a flame is detected near the remote sensor via a network connection, the system triggers a series of actions, including activating lights and buzzers as well as sending a distress message to the user's phone using IFTTT (If This Then That). The alarm can also be manually halted by pressing and holding a physical button.

Features
Flame Detection: The system can accurately detect the presence of flames through the flame sensor.

Alert Mechanism: Lights and buzzers are activated upon flame detection, providing a visual and audible alert.

IFTTT Integration: In the event of a fire, a distress message is sent to the user's phone via IFTTT, ensuring prompt notification.

Manual Control: Users can manually halt the alarm by pressing and holding a button connected to the Raspberry Pi's GPIO.

Project Structure
README.md: The project's documentation.
flame_sensor.py: Python script for interfacing with the flame sensor.
gpio_controller.py: Python script to control the GPIO pins.
app.py: The main Flask application for the web interface.
templates/: HTML templates for the web pages.
static/: Static files (CSS, JavaScript, images) for the web interface.
Getting Started
To set up the fire alarm system on your Raspberry Pi, follow these steps:

Hardware Setup: Connect the flame sensor and any additional components to the Raspberry Pi's GPIO pins as per the hardware documentation. 

   Raspberry Pi (GPIO Pins)
       │
       │
       │  Jumper Wires
       ▼
   KY-026 Flame Sensor
       │
       ▼
    Solderless Breadboard
       │
       ▼
     Red LED (+) ────┐
     Green LED (+) ──┐│
                    ││
     Jumper Wires    ││
                    ││
       │            ││
       ▼            ││
     Buzzer (─)─────┘│
       │              │
       ▼              │
     Button            │
       │              │
       ▼              │
     Resistor         │
       │              │
       ▼              │
     NodeMcu-ESP8266  │
                      │
                      ▼
                   Power Source



Software Setup: Install the required libraries and dependencies (IFTTT,Akesel,Python Flask).

Configuration: Configure the IFTTT integration, including the necessary API keys.
git repo: https://github.com/Bunker-Inc/gc23_project.git

Usage
To use the fire alarm system:

Power on the Raspberry Pi.

Ensure that the flame sensor is correctly positioned in the monitored area.

Access the web interface through a browser.

Use the engage/disengage button on the web interface to arm and disarm the security system.

In the event of a fire, the system will activate the alarm, and a distress message will be sent to your phone.

Web Interface
The web interface provides a user-friendly dashboard with an engage/disengage button to control the security system. It also includes project information and a contact page for further assistance.

Contact
SAMUEL ASUO BAFFOUR GYIMAH :
 https://instagram.com/mrtonyelvis 
Georgina Tatra:
 https://www.linkedin.com/in/georginatatra 
Isaac Ansah Neizer:
 https://www.linkedin.com/in/isaac-neizer-b06b4423b 
Jeremiah Greene:
 jerrygreene010@gmail.com


Technologies Used
Raspberry Pi
KY-026 Flame Sensor
GPIO (General-Purpose Input/Output)
Python
Flask Framework
HTML, CSS, JavaScript
IFTTT
Jumper Wire
Solderless Breadboard
Resistor
NodeMcu-EPS8266
LEDs
Buzzer

