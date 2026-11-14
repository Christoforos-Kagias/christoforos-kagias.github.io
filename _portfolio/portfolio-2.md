---
title: "Hyperion Flight Computer"
excerpt: "Design of the flight computer for Hyperion, a high-power rocket developed by the Aristotle Space and Aeronautics Team (ASAT), as part of the university's Rocketry Project.<br/><img src='/images/Flight Computer-3D model-top.png' width='400' height='400'>"
collection: portfolio
---

The project involved the design and development of the flight computer for Hyperion, a high-power rocket developed by the Aristotle Space and Aeronautics Team (ASAT).

The flight computer is responsible for collecting and recording flight data, monitoring the rocket's motion and altitude, and providing the activation signal for the recovery system.

The system is based on an STM32F030CCT6 microcontroller and integrates several peripheral devices:

- **MPU-6500:** Accelerometer used for monitoring the rocket's motion.
- **BMP280:** Barometric pressure and temperature sensor used to collect flight data.
- **SD Card:** Primary storage for recording sensor data during flight.
- **External FLASH Memory:** Redundant storage in case of SD card malfunction.
- **Voltage Regulators:** Power conversion from 9V to 3.3V for the electronic components.

Communication between the microcontroller and the external devices is implemented through SPI interfaces. The design also provides SWD connectivity for programming and debugging, as well as UART interfaces for potential future extensions.

The flight computer also interfaces with the recovery system. Based on flight parameters such as speed, altitude and time, it determines when to send the activation signal for the parachute deployment mechanism.

An important part of the development process was evaluating previous design iterations and addressing their limitations. These included insufficient microcontroller memory, the lack of redundant data storage and an SD card interface design issue. The revised design introduced a more capable microcontroller, external FLASH memory and the necessary circuit modifications.

My involvement included the design, assembly and testing of the flight computer as part of the ASAT avionics team.