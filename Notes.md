# Random Notes

### Changes
- CANTalon is it's own library
	- http://www.ctr-electronics.com/hro.html#product_tabs_technical_resources
	- Note on non-Windows: A separate package (zip) is provided to get the Talon SRX and Pidgeon libraries on non-Windows systems. Users should unzip this file and place the contents into USER\wpilib\user
- OpenCV is official library for Vision
	- Everything that we ran on the Raspberry Pi now runs on the roboRIO
	- GRIP
- WPILib is now open-source
- Joystick stuff?
	- Xbox Controller Class
- USB serial devices
- Tasks are replaced with threads
- FRC Namespace
	- Shim exists to prevent breaking until 2018
- Delay stuff has been removed
	- Replace with std::chronos

### Software Suites
- Driver Station Suite (Windows)
- Development Suite (Windows/Ubuntu)
- Simulation Suite (Ubuntu)

### Tasks
* Configure driver station
* Install canTalon libraries
* Image roboRIO according to [this](https://wpilib.screenstepslive.com/s/4485/m/13503/l/144984?data-resolve-url=true&data-manual-id=13503)
* Program radio according to [this](https://wpilib.screenstepslive.com/s/4485/m/13503/l/144986?data-resolve-url=true&data-manual-id=13503)
* Update all the firmwares as described [here](https://wpilib.screenstepslive.com/s/4485/m/13503/l/599690-updating-and-configuring-pneumatics-control-module-and-power-distribution-panel)

### mDNS Network Configuration
* roboRIO USB: 172.22.11.2
* roboRIO mDNS: roboRIO-####-FRC.local (where #### is your team number with no leading zeroes) You should be able to use this address to communicate with the roboRIO over either interface through ping, browser, etc.
* Robot Radio: 10.TE.AM.1 (where TE.AM is your 4 digit team number with leading zeroes if required)
* roboRIO Ethernet: DHCP, assigned by the Robot Radio
* Driver Station PC: DHCP, assigned by the Robot Radio
* Additional Programming computers: DHCP, assigned by the Robot Radio
* DHCP range: 10.TE.AM.20 to 10.TE.AM.199

### Static Network Configuration (Probably our best bet for field-pit consistency)
* DAP1522 radio - Static 10.TE.AM.1 programmed by Kiosk
* roboRIO - Static 10.TE.AM.2 would be a reasonable choice, subnet mask of 255.255.255.0 (default)
* Driver Station - Static 10.TE.AM.5 would be a reasonable choice, subnet mask **must be 255.0.0.0**
* IP Camera (if used) - Static 10.TE.AM.11 would be a reasonable choice, subnet 255.255.255.0 should be fine
* Other devices - Static 10.TE.AM.6-.10 or .12-.19 (.11 if camera not present) subnet 255.255.255.0