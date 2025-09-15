Done for UToronto Formula Electric Team


**Project Summary and Requirements**

Summary: the cooling loop is responsible for maintaining the temperature of two critical components of the car: the motor and the inverter. Both of these devices heat up while the car runs due to inefficiencies in the powertrain. The conversion of electrical energy to mechanical energy is not ideal with some of it (roughly 10-15%) being lost as heat. In a system that can reach up to 80kW of power, this means that as much as 12kW could be dissipated as heat! There are several key components to keeping the cooling loop running. The first are two pumps that force water through the loop. The second are the radiators (one on either side of the car) with fans that cool the water. The final elements are the sensors: sensors are integrated to the coolant loop that monitor water flow rate, pressure and temperature.

Requirements
	The goal of this project will be to design a board that accomplishes the following:

Powers and reads the cooling loop flow rate and temperature. There are two of each of the below sensors on the cooling loop:
Flowrate
Pressure
Temperature
Note that these sensors require power voltages different from 12V
Controls the cooling pumps (CAN controlled)
Datasheets for each pump found here and here
The PCB only needs to control the cooling pumps, you can assume they have their power supplied externally
Controls the radiator fans using a high side driving circuit
Note that the radiator fan power signal comes from a separate 16V bus and does not count towards the PCB power limit
Controls a relay that opens the shutdown circuit in case of a failure in the cooling loop 
The relay should be normally open
The PCB should incorporate an onboard thermistor that can measure the temperature of the board itself

The PCB must fit on a 10 x 15 cm2 rectangle
The PCB should include connectors that are waterproof
The PCB must only be powered by a 12V bus and must draw less than 1 amp peak
The PCB must use the Teensy 4.1 Microcontroller
The PCB should account for potential noise in received signals
The PCB should protect against potential failures (reverse polarity to main power, esd, etc…)
The PCB must be a four layer board
