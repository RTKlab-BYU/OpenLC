# OpenLC

This package lets you configure systems containing Zaber motors, microcontrollers, Opentrons OT2 motors, Opentrons OT2 tempdecks. 
The microcontroller's GPIO pins can be configure to operate as relays and to operate Vici valve actuators, as well as to act as generic inputs/outputs.




## Requirements
-	 Python 3.10 (3.11+ not currently supported)
  
## Optional
-	I run inside VSCode (a source code editor). After setup, virtual environment should always automatically activate for this repository
-	Other source code editors should also work fine, setup may vary slightly

## Setup
  1)	Install Python 3.10  
  2)	Make the repository location the current working directory
  3)	Run the following code:
   
      a.	Windows:
            python3.10 -m venv .venv
            .venv\Scripts\Activate
            pip install -r requirements.txt
  	
      b.	macOS/Linux:
            python3.10 -m venv .venv
            source .venv/bin/activate
            pip install -r requirements.txt

## Running
If using terminal:

  1)	Activate the virtual environment:

    	a)	Windows:
            .venv\Scripts\Activate

    	b)	macOS/Linux:
            source .venv/bin/activate
  
  2)	run the main file:

    	a)	Windows/macOS/Linux:
    	      python main.py

If using VSCode:
  1)	Run the main file:

    	a)	Windows/macOS/Linux:
            main.py



## Microcontrollers
This package contains embeded code for both arduionos and esp32-wroom-32 chips. The authors use esp chips in applications, the arduino code may not be up to date.
For either option, the microcontroller code files embeded in this repository are not run directly by package. They need to be copied to the chosen microcontroller's IDE to be flashed onto the microcontroller before configuring the main system.




https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers for WROOM driver
choose esp32 dev module
