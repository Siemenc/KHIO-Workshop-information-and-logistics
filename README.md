# CNC workshop & logistiscs KHIO
This Github page will describe how to use the MultiCam 3000 router at KHIO and help solve common errors or problems.

![Multicam 3000](https://github.com/Siemenc/KHIO-Workshop-information-and-logistics/blob/master/Images/IMG_20200124_090637.jpg)

## Machine remote:
The multicam 3000 is controled using a remote, hanging on the wall next to the router.
The machine remote is needed to control and calibrate the machine and to actually run the files.
![Machine remote](https://github.com/Siemenc/KHIO-Workshop-information-and-logistics/blob/master/Images/IMG_20200124_090555.jpg)


## Startup procedure:
- Turn on machine using the switch in the back of the machine
- Hard home the machine by pressing Shift (arrow up) first and then the button in the top left corner. There cannot be any tool inside the spindle before homing.
- Run spindle warmup routine (The remote will ask automatically after hard homing)
- Manually home the machine in X and Y direction by moving the spindle to the correct position by eyeballing and then pressing the button in the top left corner showing the 2 dots and the rectangle.
- For setting the Z-position, move the spindle down until you're close to the top of the surface. Change the speed setting to the slowest using the double arrow button on the remote. Now move the spindle in both X and Z direction until the bit scrapes the material. Now press the button to set this position as a new Z-home position (on the left?)



## Fixing material to the machine:
The multicam at KHIO uses a vacuumbed to hold most materials in place. This has advantages and disadvantages over screwing down your material to the sacraficial layer.
Advantages:
No need to screw down; No need to leave as much space around the parts to be cut out

Disadvantages:
- Vacuum leaks when milling a lot of slots
- No easy way to lign up the material along the axis


## Moving the machine:
Check which speed the machine is set to for jogging on the screen of the remote. If you'd like to switch the speed setting, press the double arrow button.
The direction of the arrows will indicate which direction the machine will move. Make sure to have the remote aligned in the correct direction of the machine (as if you're standing in front of the machine)
The normal arrows will move the machine in the x and y-direction. For moving in the z-direction

## Starting the extraction:
Automatic? Or with the switch on the machine. Currently (January 2020) it's not working.


## To start a job:
- Make sure you went through the startup procedure (turn on machine, zeroing, warm up routine)
- Make sure the correct milling bits are in the correct place of the automatic toolchanger.
- Make sure the computer is turned on and the correct file is in the correct folder
- Load a job by pressing the button showing the machine connected to a computer by cable, in the bottom left corner
- Choose which file you want to run & press enter (?)
- Turn on the vacuum
- Press the "Start" button (video cut icon)
- You'll get a preview of the job. If this looks correct (Also check by holding the remote in the correct direction according to the machine)


## Preparing toolpaths using RhinoCam



## Maintenance
- Smear grease using the grease pumps
- Check the level of the cooling water
- Refill cooling water


## Errors
