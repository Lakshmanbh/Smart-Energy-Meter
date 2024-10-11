# Smart-Energy-Meter

This project focuses on the design and development of a Smart Energy Meter, integrating modern microcontroller technology and IoT capabilities to provide real-time energy consumption data. The smart meter is designed to monitor electrical usage and provide consumers with daily energy consumption reports via SMS, helping to promote energy efficiency and transparency.

Features
Real-time monitoring of voltage, current, power, and energy consumption.
Daily energy consumption reports sent via SMS using the GSM module.
Automatic calculation of energy costs based on predefined tariffs.
LCD display to show real-time data locally.
Anti-tampering system to protect the Arduino code from unauthorized access.
Energy conservation insights to help consumers reduce usage.
Components
Current Sensor (SCT-013): Measures AC current non-invasively up to 100 amperes.
Voltage Sensor (ZMPT101B): Measures AC voltage.
Arduino UNO: Acts as the microcontroller to process data from the sensors and calculate energy consumption.
GSM Module (SIM800L): Sends daily SMS with energy usage details to the consumer's mobile phone.
Circuit Diagram
Refer to the circuit_diagram.png for the full circuit layout of the Smart Energy Meter. It includes connections between the Arduino UNO, sensors, and GSM module.

Setup and Installation
Hardware Setup
Connect the current sensor (SCT-013) to the load line to measure current.
Connect the voltage sensor (ZMPT101B) across the supply line to measure voltage.
Wire the sensors to the analog input pins of the Arduino UNO.
Connect the GSM Module (SIM800L) to the Arduino to send SMS.
Power the system using an appropriate voltage supply.
Software Installation
Clone the repository:
bash
Copy code
git clone https://github.com/yourusername/smart-energy-meter.git
Open the project in the Arduino IDE.
Install the required libraries:
EmonLib for energy monitoring.
LiquidCrystal for the LCD display.
Upload the code to the Arduino UNO via USB.
Code
The Arduino code calculates the real-time power and energy consumption and sends daily reports via SMS. The code uses:

Voltage and current calibration to measure accurate power usage.
A tariff system to calculate the cost based on energy consumption.
Usage
Once powered, the system will start monitoring voltage and current.
The energy consumption data is displayed on the LCD in real-time.
Every 24 hours, an SMS with the consumption details (in kWh) and the corresponding bill amount is sent to the consumer.
Block Diagram
Refer to the block_diagram.png for a high-level view of how the system components interact.

Future Scope
Smart Grid Integration: Use cloud-based data storage and prediction algorithms for more efficient energy management.
Wi-Fi-enabled meters: For remote control of appliances and integration with other smart home systems.
Prepaid energy meters: Allow customers to pay for energy in advance, eliminating billing disputes.
Conclusion
This smart energy meter system provides a modern solution for energy monitoring and billing transparency. By providing consumers with real-time data and insights into their energy consumption, it helps reduce energy costs and promotes sustainable energy use.

References
"Design and Development of Smart Energy Meter" by Rithesh P. Karkera, Abhishek S. Athalekar, Shubham R. Mane, Ikjot Singh Chhachhan
Various technical sources on energy monitoring systems and IoT technologies.
