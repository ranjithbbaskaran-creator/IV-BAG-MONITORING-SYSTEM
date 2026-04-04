The IV Bag Monitoring System is a smart healthcare solution developed to automate the monitoring of intravenous (IV) fluid levels and ensure patient safety. In traditional hospital settings, IV bags are manually checked by nurses, which can be inefficient and may lead to critical issues such as empty IV bags, backflow of blood, or incorrect fluid administration. This system addresses these challenges by providing continuous and real-time monitoring.
System Overview
The system is built using an Arduino-based microcontroller integrated with a load cell sensor, HX711 amplifier module, LCD display, and a buzzer alert system. The IV bag is placed on a load cell, which measures its weight continuously. Since the weight of the IV bag decreases as fluid is administered, the system uses this data to estimate the remaining fluid level.
Working Principle
When the system is powered on, it initializes all components and performs a basic system check. Once activated, the load cell starts measuring the weight of the IV bag and sends this data to the Arduino through the HX711 module.
The Arduino processes the incoming data and displays the real-time weight on the LCD screen. Predefined threshold values are set within the program:
•	Normal Level: System operates without alerts 
•	Low Level: When the fluid drops below a certain limit, a warning message is displayed and the buzzer produces intermittent alerts 
•	Critical Level: When the fluid level becomes dangerously low, the system triggers a continuous alert indicating immediate attention is required 
If any abnormal readings (such as negative values) are detected, the system identifies it as an error and notifies the user via the display.
Key Components
•	Load Cell: Measures the weight of the IV bag 
•	HX711 Module: Amplifies and converts sensor data for Arduino 
•	Arduino Uno: Acts as the main controller and processes data 
•	LCD Display (16x2): Shows real-time weight and system messages 
•	Buzzer: Provides audio alerts for low and critical levels 
•	Push Button: Used to start or control the monitoring process 
Features
•	Real-time monitoring of IV fluid levels 
•	Automatic alert system for low and critical conditions 
•	Error detection and indication 
•	Simple and cost-effective design 
•	Reduces manual supervision by healthcare staff 
Advantages
•	Improves patient safety by preventing empty IV conditions 
•	Minimizes human error in monitoring 
•	Saves time for medical staff 
•	Provides reliable and continuous observation 
Conclusion
This system offers an efficient and practical solution for monitoring IV fluid levels in healthcare environments. By combining sensors and automation, it ensures timely alerts and enhances the quality of patient care while reducing workload on medical staff.

