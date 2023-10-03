# Gas-sens_Rs-485
a Compact, cheap gas sensor with RS-485 connectivity

## Concept:
24V supplied, Gas detector with half-duplex RS-485 interface. For industrial or home use and application ready product, containing a current or voltage output for reference measurment.
a sinlge LED used for showing cominucation or Error state. The small footprint makes it ready for most plastic enclosures.
the PCB can be hand-solderd with a bit of skill. 
Use cases can be in Garage systems (linked with the vents and gas alarm system), hobbyist workshop or any other room such as Office spaces and schools.

![front-view](/Pictures/3d_Top.PNG "front-view")
![back-view](/Pictures/3d_Bottom.PNG "back-view")

## Components

A STM32G031K8 is the logical unit. Is is cheap and readily available.
The very most components use standart fooprints. Thus, they are easily exchangeble in case of a shortage.
All parts are SMD, except for the Sensors, DCDC converter and Connectors.
All PCB components can be sourced by Mouser, except for the Gas Sensor.
for developement purposes (TAG v0.1) a gas sensor type MQ-X were used (MQ-7 and MQ-135)
i am currently looking into more professional solutions for the sensor.

## Programming
Hardware is developed in KiCad 7.0.
everything is programmed on STM Cube IDE. The Sensor and trim potentiometers are read-in using DMA

## Simulation
Low pass filter for the PWM (from uC to OpAmp to voltag eand current output) has been simulated using LTSpice.

## next steps
[x] PWM filter simulations
[x] build and test prototype
[x] Prgram IC for analog measurment and analog output
[] Find better sensor supplier and include it on second version PCB
[] implement Modbus via RS-485
[] create Bill of material
[] Make second physical prototype
