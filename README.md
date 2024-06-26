# S.P.A.R.K

The repository contains the necessary operational code for the Strategic Pyro Assault Rescue Kinetic - S.P.A.R.K.
It is a mobile firefighting automaton which detects, approaches, and extinguishes localized fires.


## Purpose
The robot was inspired by the problem of fire incidents in server rooms and data centers. Even a small fire in such a high-stakes location causes service disruption costing companies assets in the millions - not to mention the potential loss of life.

## Current Solutions
Present fire suppression systems include:
- Water Cannons
  Flaw: Large scale water damage to high cost equipment, irretrievable data losses
-  Clean Agent Supression:
  Flaw: Harmful to humans, requiring evacuation, thus service disruptions potentially costing millions

## Our Solution
*S.P.A.R.K*: An atonomous mobile firefighting robot designed to extinguish small-scale localized fires with minimal water damage, no need for evacuation, thus reducing service disruptions, data loss, and costly equipment replacement.

## Files
The files contain code for sensor-activation and actuator-response for the following components:
- IR/Ultrasonic Flame Sensors: To detect the presence of fire.
- Ultrasonic Sensors: To avoid obstacles when the robot is mobile.
- Microservo: To adjust the height of the turret in the vertical plane
- Unipolar Stepper Motor: To rotate the turret at a precise angle to aim at the flame.
- DC Pump: To pump water from storage to the hose in the turret to extinguish the fire when detected.
- Drivers: To control the wheels of the mobile base.

## Requirements and Compatibility
- Hardware Requirements: Raspberry Pi, Raspberry Pi Pico
- Software Software Requirements: Micropython, ROS2 is required for effective communication and successful implementation.
- Additional Packages and Libraries: import rclpy, from rclpy.node import Node, import time, import lgpio, import serial, from std_msgs.msg import String
  (Please note that the ROS2 code was run on VSCode on a Linux Raspberry Pi requiring the use of lgpio. If you are running the code on a different piece of software then I recommend changing the package to match your system)
- Rename navigation.py to main.py to run it on pico without cable.

