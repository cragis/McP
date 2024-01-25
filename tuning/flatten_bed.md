# McP Tuning: Frame check


## Step 1: Supplies

These are the supplies you need

1. 3D Printer
1. tools

## Step 2: Check screws
Test the screws and nuts around the printer to make sure they are all tightened.  Also check that the aluminum extrusions are perpendicular to each other at each connection.

## Step 3: Check belts and pulleys
1. Verify that your belts all have enough tension, but not too much.  With the correct amount, you can pluck the full length run of the belt and get hear a low frequency musical note.  Typically 90 Hz is a good frequency.
1. Verify that pulleys are tightened onto their shafts trying to move the belt while holding the flat of the shaft with pliers.  The belt should not be able to move without turning motor shaft.
## Step 4: Align trapezoidal nuts

1. Perform a z-axis auto-align.
1. Release the tension on the X smooth rods by unscrewing the tensioning M3x10 screws (those near the top and bottom of the right end of the idler) a few turns. (Note! These are different from the X axis belt tensioning screws.)
1. Relax the tension of the X axis belt.
1. Loosen the screws which secure the (black delrin) trapezoidal nuts. This is to ensure that the trapezoidal nuts 'self-center' on the lead screws.
1. Make sure the trapezoidal nuts are able to move freely.
1. Alternating between all 4 screws, incrementally tighten each screw to secure the trapezoidal nuts (alternate between both sides during this process). Don't apply any lateral force to the trapezoidal nuts.




## Step 5: Fine tune x-axis length
1.  To adjust the length of the X axis we use the two M3x10 screws of the x_end_idler while looking at the Z tops.

1. While you tighten the M3x10 screws keep an eye on the Z tops. The M3x10 screws will move the Z lead screws laterally (left or right), adjust them so that the Z lead screws are centred.
1. Re-tighten the x-axis belt.
Note that the M3x10 screws will not move the lead screws forwards or backwards, only laterally.

## Step 6: Lubricate
1. Put a drop of oil on each of the linear rods that make the x-axis.
1. Move the axis through its whole motion several times so that the bearings spread the oil along the whole rod and into the bearings.
1. Repeat with y-axis.
1. Repeat with z-axis.  (Double-clicking from info screen is a quick way to get to control of z-position in the software.) 

## Step 7: Check extruder and nozzle
Verify that the extruder is held securely and that the nozzle is tight.  If nozzle needs tightening, it should be done at operating temperature (~240 degrees celsius).
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
