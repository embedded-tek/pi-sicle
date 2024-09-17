# pi-sicle Development Board
Examples and Settings for pi-sicle  FPGA development board.

## Firmware
The pi-sicle development board will ship with the newest firmware as of the date of shipment. If the board becomes unresponsive or is not operating appropriately, download and flash the lastet firmware.
### Installing the Firmware
- Download the lastest UF2 file the firmware folder
- Bridge the `USB_Boot` pins on the top side of the board
- Connect the pi-sicle board to a computer
- USB drive should populate
- Copy and paste the UF2 to the drive
The board should now auto unmount and reset. The baord is now flashed with the latest firmware!

## Loader Application
In order to upload a bitstream to the pi-sicle development board, a loader application is required. The loader application found here is a pip module which is easily installed/updated.
- Download the latest version of the loader
- If using a virtual environment, activate the environment used with the pi-sicle board
- Navigate to the directory downloaded from here
- Unzip/untar the directory and change into it
- If this is a new installation run: `pip install *.tar.gz`
- If updating an existing installation, run: `pip install --upgrade *.tar.gz`
The installer should now be a callable commandline program via: `pi-sicle-loader`. Test the module by running: `pi-sicle-loader --help`. If the arguments list is not printed, try restarting the terminal/PowerShell session and running the module again. 
