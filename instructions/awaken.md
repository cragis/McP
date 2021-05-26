# McP StartUp instructions


## Step 1: make a print sheet

you cannot print directly on the belly (heated bed).  You will need to affix a print sheet on top of it.

Cut a glass or mirror plate to fit the heated bed (244mm x 254mm).  If you use a bare glass bed, there are a number of glues that can be used to give good adhesion: dilute elmer's wood glue, hairspray, layerneer,   ...
 
Optional: Make a PEI covered print bed
Take your print sheet and a piece of PEI to attach to it.  Clean the sheet as well as you can before applying the plastic.

Here is a video that shows one way to apply the PEI: [PEI attachment] (https://www.youtube.com/watch?v=Zg9LDfDJrDc)

A credit card or similar squeegee can help apply smoothly.

Affix the print sheet to the belly using binder clips.  Remove the handles once the clips are attached.

## Step 2: Turn on

Plug your machine in.  Turn on the switch.

:warning: Often LCDs come with the key on the connectors reversed.  If your LCD does not light up when you first turn on your printer, this is likely the problem.  Turn off the printer.  Now remove the black housing on the electrical connector by carefully prying it off of the board.  Reverse the connector. Reapply it.


## Step 3: Explore menus

Try navigating around the menus by turning and pushing the knob.  Try to remember some of the possible selections.

## Step 4: Testing 

If the testing fails at any point, reset your printer (the button marked X).  Then work to identify and fix the error.

### Test axes

1. Navigate to move x-axis by 10 mm steps (Prepare/Move axis/Move X/Move 10mm).
1. Turn the knob one click clockwise.  Hand (hotend assembly) should move 10 mm right.
1. Turn the knob one click counterclockwise.  Hand should move back to where it started.
1. Do the same steps for the y-axis.  Bed (belly) should move forward and backward instead.
1. Do the same steps for the z-axis.  Hand should move up and down.

### Test endstops

1. Find "Auto home" (Motion/Auto home) in the menus and execute it.  
1. The hand will move left first, press reset if motor doesn't stop when x-endstop is reached.
1. Next, the bed will move backward. Press reset if motor doesn't stop when y-endstop is reached.
1. Now the hand will move down. Prepare to press reset if the nozzle gets closer than 0.5mm to the bed.  DO NOT LET THE NOZZLE CONTACT THE BED!

### Add Filament. Test heaters, thermometers, and extruder. 

1. Select "Preheat PET" (Temperature/Preheat PET/Preheat PET).
1. When the temperature of the extruder is above 230 degrees celsius, select "Change Filament" (Prepare/Change filament).  Select a roll of PETG filament and load it when instructed.
1. Using tweezers, clean any filament off the nozzle.

## Step 5: Measure bed plane

1. Wait until bed temperature is at target (70 degrees celsius).
1. Make x-axis level by running AutoZ-Align(Motion/AutoZ-Align)
1. Run Bed Leveling mesh measurement (Motion/Bed Leveling/Level Bed).
1. Watch to see that nozzle never touches bed.  Procedure will finish in about 10 minutes.
1. Store measured bed mesh (Configuration/Store settings).

## Step 6: Z-offset adjust

The sensor will trigger with the nozzle a short distance above the bed.  Now we will manually adjust this to get the height offset correct for your machine.

1. Start a print.
1. Wait for printer to warm, the nozzle to auto-home and park at the front left of the bed at a nominal height of 0.1 mm.
1. Slowly double-click the knob (only works while a print is in process) to bring up the "Probe Z Offset" function.
1. Adjust the setting until the nozzle is close to but not touching the bed.
1. The print will start soon.
1. Try to adjust the z-offset to get the first layer adhering well and quite smooth.  The bead formed should be somewhat flattened between the bed and the nozzle. 
![](img/first_layer_crosssection.png)\
The filament bead should be shaped like this.
1. The layer formed should be connected and quite smooth, so keep adjusting as necessary.
![](img/NozzleTooHigh.jpg)\
Offset not negative enough
![](img/NozzleTooLow.jpg)\
Offset too negative
![](img/NozzleHeightPerfect.jpg)\
Offset in Goldilocks zone
1. Repeat Z-offset adjust as necessary.

You can do this adjustment on the first layer of any print to improve first layer quality.  First layer quality is the most important part of making successful prints.

## Step 7: IMPORTANT! Save settings.

Store settings (Configuration/Store settings) to remember (even after reset) your bed mesh and z-offset adjustment.

## Step 8: OPTIONAL Measure extrusion

You may need to measure if your extruder is extruding the amount of filament that it thinks it is.

1. Preheat for PET and wait until temperature is reached.
1. Make a sharpie mark on the filament about (precision not necessary) 10cm (100mm) above where it enters the extruder.
1. Using calipers, measure the distance along the filament from the top of the extruder to this mark. Record this value. (Precision is necessary.)
1. Go to the setting to move the extruder axis by 10mm steps.
1. Turn the knob one tick clockwise to extrude 10mm of filament.
1. Once the extruder stops turning, measure and record the distance again.
1. Repeat until your mark disappears into the extruder.

If you now make a plot of expected position (0mm, 10mm, 20mm, 30mm, ...) vs. your measured length, the slope will be the factor by which you should multiply the extruder calibration.  Ask for help if you need it. 


## Step 9: Other

There are a few things that are not complete.  In order to use the extrusion cooling fan, you need to print and attach a fan shroud. Many useful designs exist, search the internet.

There will likely be many improvements you can make to the calibration or performance of the machine.  Play around yourself and read about the experiences of others.

  
#### [Previous Step: brain](brain.md) &nbsp;&nbsp;&nbsp; [Next Step: enjoy]
