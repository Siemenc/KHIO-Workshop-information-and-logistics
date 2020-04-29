# CNC workshop & logistiscs KHIO
This Repository will describe how to use the MultiCam 3000 router at KHIO and help solve common errors or problems.

![Multicam 3000](https://github.com/Siemenc/KHIO-Workshop-information-and-logistics/blob/master/Images/IMG_20200124_090637.jpg)

## Machine remote:
The multicam 3000 is controled using a remote, hanging on the wall next to the router.
The machine remote is needed to control and calibrate the machine and to actually run the files.
![Machine remote](https://github.com/Siemenc/KHIO-Workshop-information-and-logistics/blob/master/Images/IMG_20200124_090555.jpg)


## Startup procedure:
- **Turn on machine** using the switch in the back of the machine
- **Hard home** the machine by pressing Shift (arrow up) first and then the green button in the top left corner. There cannot be any tool inside the spindle before homing. If there is a tool in the spindle go to "Errors" below.
![Hard Home](https://github.com/Siemenc/KHIO-Workshop-information-and-logistics/blob/master/Images/HardHome.jpg)
- Run **spindle warmup routine** (The remote will ask automatically after hard homing)
- **Manually home the machine in X and Y according to the material** you are cutting: move the spindle to the correct position by eyeballing and then pressing the blue button on the left showing the 2 dots and the rectangle.
![Home](https://github.com/Siemenc/KHIO-Workshop-information-and-logistics/blob/master/Images/Home.jpg)
- **Manually home the machine in Z according to the material**: move the spindle with the milling bit down using the Z movement buttons until you're close to the top of the surface you are milling. Change the speed settings to the slowest using the double arrow button on the remote. Now move the spindle in both X and Z direction until the bit scrapes the material. Now press the blue button on the left as shown below to set this position as a new Z-home position.
![HomeZ](https://github.com/Siemenc/KHIO-Workshop-information-and-logistics/blob/master/Images/HomeZ.jpg)


## Fixing material to the machine:
The multicam at KHIO uses a vacuumbed to hold most materials in place. The vacuumbed is divided into 4 section which can be turned on/off using the handles in the front. Having a vacuumbed has advantages and disadvantages over other machines where you screw down your material to the sacraficial layer (f.e. Shopbot @ Fellesverkstedet).

Advantages:
- No need to spend time screw down and taking screw into consideration when creating toolpaths
- No need to leave as much space around the parts to be cut out

Disadvantages:
- Vacuum leaks when milling a lot of slots
- No easy way to lign up the material along the origin
- In case your piece is smaller than the section of the vacuumbed, you need to cover the rest of the section to prevent leaking of the vacuum.

## Moving the machine:
Check which speed the machine is set to for jogging on the screen of the remote. If you'd like to switch the speed setting, press the double arrow button.

The direction of the arrows will indicate which direction the machine will move. Make sure to have the remote aligned in the correct direction of the machine (as if you're standing in front of the machine)
The normal arrows will move the machine in the x and y-direction. For moving in the z-direction you press

## Starting the extraction:
Automatic? Or with the switch on the machine. Currently (January 2020) it's not working.

## To start a job:
- Make sure you went through the startup procedure (turn on machine, zeroing, warm up routine)
- Make sure the correct milling bits are in the correct place of the automatic toolchanger.
- Make sure the computer is turned on and the correct file is in the correct folder
- Load a job by pressing the button showing the machine connected to a computer by cable, in the bottom left corner
- Choose which file you want to run & press Enter (button in bottom left corner)
- Turn on the vacuum
- You'll get a preview of the job. If this looks correct (Also check by holding the remote in the correct direction according to the machine) you can press the "Start" button (video cut icon)

## To check how much time the last job took
- Using the machine controller: press the menu button
- Go to Utilies using the down arrow button and press the Enter button
- Go to ... to be continued...

## To restart the last job from a certain position:
- Move the bit close to the physical position from where you would like to start. (Usually you restart the last job after something went wrong, the job got cancelled or interrupted.)
- Press Shift (1) and then Start (2)
- Now the machine will find the closest points to your current position and you'll have the option to choose whether you start from there by pressing the "Start" button, or go to the next closest point by pressing the arrow downwards.
![Restart](https://github.com/Siemenc/KHIO-Workshop-information-and-logistics/blob/master/Images/Restart.jpg)


## Preparing toolpaths using RhinoCam


## Postprocessing toolpaths


## Maintenance
- Refill grease using the grease pumps
There's 13 nipples on the machine to feed the grease into:
- 4 on the X-axis (2 on each side of the bridge)
- 4 on the Y axis (2 on each side of the Z-axis)
- 5 on the Z-axis (2 on each side of the Spindle and 1 on the top to grease the screw controlling the Z-axis)
Make sure the grease pump clicks on the nipple before trying to pump grease. You might need to push the connector onto the nipple to make sure the grease-container gets filled and the grease doesn't spread around the nipple. If you can see the grease coming out onto the guide (not next to the nipple!) you've done it correctly.

- Check the level of the cooling water

- Refill cooling water

- Clean filter of vacuum-bed
On the left side of the machine there's a machine colored black with orange details. This is the machine creating the vacuum for the machine bed. On top of the machine there's a black cylinder where a blue tube runs into. This is the filter container. Make sure the vacuum bed is not on and unlock the clamps on the front of the filter container. Inside this container you will find the filter which you can just take out. Use compressed air to blow the dust out of the filter by blowing from the hole in the center to the edges of the filter. Also clean out the black filter cabinet from any dust as this otherwise would get sucked back into the filter.

## Calibrating the tool
Until instructions are written down, check out this link: https://www.youtube.com/watch?v=kye__44Uw2s


## Errors
- Low Air Pressure: The machine won't unload or load a tool and will not start a job. Last time this happened (January 2020), this got fixed by replacing the filter of the compressed air. To do this you'll need a new filter. Replace the hold filter by first cutting off the flow of air coming into the filter using the lever at the ceiling. Then follow the instructions that come with the new filter. Last time the 3rd filter (the one most on the right) when looking at the wall with the filters got replaced.
- Modbus Timeout Slv:14: Error that randomly pops up together with "80000 Error occured". We don't know what causes this but usually you can continue using the machine and perhaps need to restart the job.
- Dus collector NOT open! (ENTER to continue): This error has popped up when trying to start a job. This got fixed by making sure the dust skirt can move upwards and hit the sensor (a red light on the top left next to the spindle). There might have been some dust clogged up that prevents hitting this switch
