## Larus Flight Information Sensor System for Gliders

This project provides hardware and software to create a **Sensor System** for **Glider Flight-Management-Systems** like [XCsoar](https://github.com/XCSoar).

Sensor hardware containing an **IMU**, **pressure sensors** and a **(D-)GNSS**

### Overview
- Documentation starting point: https://github.com/larus-breeze/doc_larus


### Sensor
https://github.com/larus-breeze/hw_sensor, https://github.com/larus-breeze/sw_sensor

![PCB](profile/PCB.jpg)
The sensor firmware is providing essential information for glider navigation like 

  - **position**, 
  - attitude and heading **AHRS**, 
  - GNSS/INS-based ultra-fast **variometer**, 
  - **real-time wind measurement**, 
  - **air-density** measurement 

  and much more.
<!--  -->
Software-In-The-Loop (**SIL**)-Simulator to test and qualify algorithms 

Experimentally: Additional sensors like Angle-Of-Attack or meteorological data

Some more details about the features can be found under [algorithms](https://github.com/larus-breeze/sw_sensor_algorithms).

The sensor can also be used as a universal data-logger for manned or UAV test flights with a sampling-rate of 100 Hz. The logger writes it's data to a micro-sd with a virtually unlimited capacity. Extra sensors can be added over the CAN bus.

![Assembled](profile/GNSS-Assembled.jpg)
**Fully assembled first unit**

![Assembled DGNSS](profile/DGNSS-Assembly.JPG)
**DGNSS (Sat Compass) Larus Sensor**



