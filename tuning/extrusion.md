# McP Tuning: Extrusion


## Step 1: Supplies

These are the supplies you need

1. 3D Printer
1. filament (loaded into printer)
1. sharpie
1. calipers

## Step 2: Preheat
Start a preheat for the filament you are using (usually PETG for me).
## Step 3: Mark filament
Make a mark on the filament about 100 mm above the top of the extruder.
## Step 4: Measure mark location
Using the calipers, measure the distance from the extruder to your mark (to the nearest 0.1 mm is good).  Record this value.
## Step 5: Move the filament 
Navigate to Settings->move axis->extruder.  Turn the knob so that the number shown increases by 10 mm
## Step 6: Repeat
Repeat steps 3 and 4 until mark is inside extruder.
## Step 7: Graph data
Make a graph of supposed distance (0 mm, 10 mm, 20 mm, etc.) vs. measured distance.
## Step 8: Evaluate data
If your points do not fall on a line, you have an inconsistent extrusion issue.  Try to fix it.

If you do find a nice line, find the slope of your graph's line.
## Step 9: Recalibrate
Your extrusion calibration (steps/mm) should be multiplied by the slope of your fit to give a better calibrated value.

The old value can be read by sending a gcode:
M503

Sending these gcode commands will replace the current value
M92 E{newvalue}
M500

[comment]: # [Previous Step: face](face.md) &nbsp;&nbsp;&nbsp; [Next Step: awaken](awaken.md)
