# Gas-sens_Rs-485
a Compact, cheap gas sensor with RS-485 connectivity

## Concept:
24V supplied, Gas detector with half-duplex RS-485 interface. For industrial application ready product, containing a current or voltage output for reference measurment.
a sinlge LED used for showing cominucation or Error state. the small footprint makes it ready for most plastic enclosures.
the PCB can be hand-solderd with a bit of skill. 
Use cases can be in Garage systems (linked with the vents and gas alarm system), hobbyist workshop or any other room such as Office spaces and schools.

![grafik](https://github.com/Sarbf1/Gas-sens_Rs-485/tree/main/Pictures/3d_Top.PNG)
![grafik](https://github.com/Sarbf1/Gas-sens_Rs-485/tree/main/Pictures/3d_Bottom.PNG)

## Components

A STM32G031K8 is the logical unit. Is is cheap and readily available.
The very most components use standart fooprints. thus, they are easily exchangeble in case of a shortage.
The parts are SMD, except for the Sensors, DCDC converter and Connectorss
All PCB components can be sourced by Mouser.

## Programming
Hardware is developed in KiCad 7.0.
everything is programmed on STM Cube IDE. The Sensor and trim potentiometers are read-in using DMA

## Simulation
Low pass filter for the PWM (from uC to OpAmp) has been simulated using LTSpice.

