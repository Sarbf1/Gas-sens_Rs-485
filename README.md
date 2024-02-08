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
For developement purposes (TAG v0.1) a gas sensor type MQ-X were used (MQ-7 and MQ-135)
TAG v0.2 makes use of the nemoto sensor, that uses low current and is more gas specific. 
The I2C conection gives a possibility, to further extend with more sensors, such as the Sensirion SHT4X.

## Programming
Hardware is developed in KiCad 7.0.

everything is programmed on STM Cube IDE. The Sensor and trim potentiometers are read-in using DMA.
The max and minimum values of the potentiometers can be set by the Modbus. the specific address are found in the excel-table "Modbus-memorymap" in the software folder.

## Simulation
Low pass filter for the PWM (from uC to OpAmp to voltag eand current output) has been simulated using LTSpice.


## next steps
- [X] PWM filter simulations
- [x] build and test prototype
- [x] Prgram IC for analog measurment and analog output
- [x] Find better sensor supplier and include it on second version PCB -> nemoto sensors
- [x] implement Modbus via RS-485
- [ ] create Bill of material
- [x] Make second physical prototype

