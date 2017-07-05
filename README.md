## IP Name ##

DMM-Switch-ScanList Custom Device

This Custom Device was developed to be used in applications where you need to use a Switch combined with a DMM to measure a significant number of channels. The Custom Device allows configuration for the Switch model and channel list as well as DMM measurement and trigger configuration.
The scanning only supports mux configurations and is hardware based (handshaking mode). Sacnned measurements work as follows:

1. Switch connects a channel
2. Switch sends trigger to DMM
3. DMM measures
4. DMM sends a trigger to the Switch
5. Switch connects to the next channel
6. Repeats from step 1 until channel list is done.
 

### LabVIEW Version ###

LabVIEW 2015 - Current source code was developed in LabVIEW 2015

### Built Availability ###

Only source-code is supplied, no built version

### Quality, Limitations ###

Quality: This is first public version of the Custom-Device.

Limitations:

- This Custom Device was developed and tested using a PXI-2503 and a PXI-4072 in a PharLap PXI controller. This Custom Device should work with all the Switch and DMM NI offering, but hasn't been tested with all the Switch-DMM combinations available.
- Only tested for PharLap.
- Voltage (AC/DC), Current (AC/DC), Resistance, and Capacitance measurements have been tested. The rest of measurements are available but have not been tested.
- This Custom Device is intended to work in ScanList mode. Individual switch connections or matrix configurations are not supported. 
- Only mux configurations are supported.
- The scanning is done in hardware using PXI triggers in handshaking mode.

### Dependencies ###

Describe any dependencies of the IP

- NI-Switch
- NI-DMM

### License ###

*This repository and any materials provided by NI therein are provided AS IS. NI DISCLAIMS ANY AND ALL LIABILITIES FOR AND MAKES NO WARRANTIES, EITHER EXPRESS OR IMPLIED, INCLUDING WITHOUT LIMITATION ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR  PARTICULAR PURPOSE, OR NON-INFRINGEMENT OF INTELLECTUAL PROPERTY. NI shall have no liability for any direct, indirect, incidental, punitive, special, or consequential damages for your use of the repository or any materials contained therein.*