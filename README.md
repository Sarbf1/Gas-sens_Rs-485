# Gas-sens_Rs-485
a Compact, cheap gas sensor with RS-485 connectivity

## Concept:
24V supplied, Gas detector with half-duplex RS-485 interface. For industrial application ready product, containing a current or voltage output for reference measurment.
a sinlge LED used for showing cominucation or Error state. the small footprint makes it ready for most plastic enclosures.
the PCB can be hand-solderd with a bit of skill. 
Use cases can be in Garage systems (linked with the vents and gas alarm system), hobbyist workshop or any other room such as Office spaces and schools.



## Components
The core is a MiCS-6814 Gas sensor. It was chosen due to the small build size, cheap price and containing a reduction (CO), Ox (zb. NO2) and NH3 sensor in one case.
A STM8S003F3P is the logical unit. Is is cheap and readily available.
Internally all components used are 5V supplied, by an oversized non isolated DC/DC converter.
All PCB components can be sourced by Mounser.

## Programs
Hardware is developed in KiCad 7.0.
Initially i wanted to programm on STM Cube IDE. currently not shure if it will work on a 8bit microcontroller.
