## Larus Flight Information Sensor System for Gliders

This project provides hardware and software to create a **Sensor System** for **Glider Flight-Management-Systems** like [XCsoar](https://github.com/XCSoar).

### Overview
- The documentation starting point is here: https://github.com/larus-breeze/doc_larus

### Frontend
- 57mm display unit. With transflective 2" display, STM32H7 and Rust firmware. 
![Frontend New Units](profile/frontend_indirect_bright_sunlight.jpg)
![Frontend New Units](profile/frontend_new_units.jpg)

### Sensor
https://github.com/larus-breeze/hw_sensor, https://github.com/larus-breeze/sw_sensor
Sensor hardware containing an **IMU**, **pressure sensors** and a **(D-)GNSS**
The sensor firmware is providing essential information for glider navigation like 

  - **position**, 
  - attitude and heading **AHRS** Heading in DGNSS Version via satellite 
  - GNSS/INS-based ultra-fast **variometer**, 
  - **real-time wind measurement**, 
  - **air-density** measurement
  - worldwide automatic adaption to the local **magnetic field parameters** using NOAA data.
  and much more.
<!--  -->
Software-In-The-Loop (**SIL**)-Simulator to test and qualify algorithms 

Some more details about the features can be found under [algorithms](https://github.com/larus-breeze/sw_sensor_algorithms).

The sensor can also be used as a universal data-logger for manned or UAV test flights with a sampling-rate of 100 Hz. The logger writes it's data to a micro-sd with a virtually unlimited capacity. The Frontend is connected via a CAN bus.

![Assembled](profile/GNSS-Assembled.jpg)
**Fully assembled unit with single GNSS**

![Assembled DGNSS](profile/DGNSS-Assembly.jpg)
**DGNSS (Sat Compass) Larus Sensor**



