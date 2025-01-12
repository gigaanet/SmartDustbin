Smart Dustbin Segregator

The Smart Dustbin Segregator is an Arduino-based project that automates the process of segregating waste into wet and dry categories and monitors the dustbin's capacity. It uses a combination of sensors and a servo motor to achieve this functionality, making waste management more efficient and hygienic
Features
Waste Segregation: Automatically distinguishes between wet and dry waste using an IR sensor and a soil moisture sensor.
Capacity Monitoring: Monitors the dustbin's capacity using an ultrasonic sensor and displays the remaining capacity on an OLED display.

Servo Motor Control: Operates a servo motor to open the appropriate compartment for wet or dry waste.

Components Used
1. Arduino Uno: The microcontroller that acts as the brain of the project.
2. IR Sensor: Detects the presence of waste near the dustbin.
3. Soil Moisture Sensor: Measures the moisture level to distinguish between wet and dry waste.
4. Ultrasonic Sensor (HC-SR04): Measures the distance to the waste in the bin to determine the bin's capacity.
5. Servo Motor: Opens and closes the compartments for wet and dry waste.
6. OLED Display (SSD1306): Displays the remaining capacity of the dustbin.
7. Miscellaneous: Wires, breadboard, and power supply.

Working Principle
1. Waste Detection:
The IR sensor detects the presence of waste near the dustbin.
Once detected, the soil moisture sensor is activated to measure the moisture content of the waste.
2. Waste Classification:
If the moisture content is high, the waste is classified as wet.
If the moisture content is low, the waste is classified as dry.
Based on this classification, the servo motor opens the respective compartment for the waste to be disposed of.
3. Capacity Monitoring:
The ultrasonic sensor continuously monitors the distance between the top of the bin and the waste.
The distance is used to calculate the remaining capacity of the dustbin.
The OLED display shows the percentage of remaining capacity.
4. Alerts:
If the dustbin is full (capacity below a certain threshold), a "Dustbin is full" message is displayed on the OLED screen.
If the dustbin is empty, a "Dustbin is empty" message is displayed.
Otherwise, the remaining capacity percentage is displayed.

Code Overview
The code consists of the following sections:
Setup: Initializes the sensors, servo motor, and OLED display. It also sets up the pins and prepares the components for operation.
Loop: Continuously reads data from the sensors, processes it to classify waste, controls the servo motor, and updates the OLED display with the current status.

How to Use
1. Assemble the Components: Connect the components as per the circuit diagram provided.
2. Upload the Code: Upload the provided Arduino code to the Arduino Uno using the Arduino IDE.
3. Power Up: Connect the Arduino to a power source or USB to start the system.
4. Operate: Place waste near the IR sensor to trigger the segregation process. Check the OLED display for the dustbin's capacity status.

Applications
Household Waste Management: Automates the segregation of waste at home.
Public Waste Bins: Can be used in public areas to promote better waste segregation and management.
Smart Cities: A component in the broader smart city initiatives for efficient waste management.
Future Enhancements
Mobile App Integration: Sending alerts to a mobile app when the bin is full.
Multiple Sensors: Integrating additional sensors for more detailed waste classification.
Energy Efficiency: Optimizing power consumption for long-term operation.

License
This project is open-source and licensed under the MIT License.
