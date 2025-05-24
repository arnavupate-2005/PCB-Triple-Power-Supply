Triple Voltage Power Supply PCB
Designed by: Arnav Upate
![image](https://github.com/user-attachments/assets/516c2eab-8a66-4221-997e-75bdd176236d)


Overview
This is a custom-designed Triple Output Power Supply PCB that provides regulated DC outputs of 12V, 5V, and 3.3V from a single DC input source. It's ideal for powering development boards, sensors, and other low-voltage electronics from one compact board.

Features
Three Regulated Outputs:

12V Output via P2

5V Output via P4

3.3V Output via P5

Input Voltage: Recommended 15V–24V DC (connected at VIN/GND terminal)

On-board LED Indicators (LED1, LED2, LED3) for each voltage rail

Screw Terminals for secure input and output connections

Heat-sinked linear regulators for stable output

Capacitor filtering on input/output for voltage stability

Components
Reference	Component	Function
U1	Voltage Regulator	12V Output (e.g., LM7812)
U2	Voltage Regulator	5V Output (e.g., LM7805)
U3	Voltage Regulator	3.3V Output (e.g., AMS1117-3.3)
C2, C3...	Electrolytic Caps	Input/output filtering
R1-R3	Resistors	Current limiting for LEDs
LED1-3	Red LEDs	Power indication per output rail
P1	Input Terminal	Connect VIN and GND
P2	12V Output	Screw terminal
P4	5V Output	Screw terminal
P5	3.3V Output	Screw terminal

How to Use
Connect DC input voltage (15–24V recommended) to the +VIN and GND terminal (P1).

The three output rails are:

P2: 12V Output

P4: 5V Output

P5: 3.3V Output

Each output rail has an associated status LED to indicate proper voltage regulation.

Be mindful of the maximum current rating of each voltage regulator.

Design Notes
Linear Regulators are used, so proper heat dissipation is required. Each regulator has a heatsink pad to handle thermal load.

Ensure adequate input voltage headroom for proper regulation, especially for 12V and 5V outputs.

Compact and clearly labeled layout makes it suitable for lab and project bench power supplies.


Safety Tips
Do not exceed regulator current ratings (typically 1A for TO-220 packages without active cooling).

Double-check polarity before applying power.

Mount the regulators to a heatsink if operating near full load


