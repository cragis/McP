# McP StartUp instructions

##  Step 1: Get the x axis accurately horizontal

1. Move the extruder to the left until in closes the x endstop switch.
1. Get a spacer, about 10 mm thick.
1. Move the extruder down by turning both threaded rods until the nozzle is just barely touching the spacer with the spacer resting on the bed.  
1. Move the extruder toward the right.  (Don't let the nozzle touch anything.  If it is getting closer to the bed, turn the right threaded rod.)
1. At far right, move the extruder up or down with the right threaded rod until the nozzle is just barely touching the spacer with the spacer resting on the bed.
1. Move the extruder back to the right and repeat until nozzle it exactly at the height of the spacer throughout the whole width of the bed.

##  Step 2: Adjust inductive sensor height

1. Loosen the screw holding the inductive sensor (the threaded cylinder with the gray bottom that is right of and behind the nozzle).
1. Adjust the height of the inductive sensor so that it is 0.6mm above the end of the nozzle.  A plastic alignment aid that has a 0.6mm step on it is helpful. 
1. Tighten the screw.
1. Make sure the lowest part of the sensor is visibly higher than the nozzle, but still less than 1mm higher.

## Step 3: Turn on

Plug your machine in.  Turn on the switch.

## Step 4: Self Test

Run the self test in the calibration menu

## Step 5: XYZ calibration

Run the XYZ calibration step in the calibration menu. This step takes about 15 minutes.  Be patient but attentive.

## Step 6: Z-offset adjust

The inductive sensor will trigger with the nozzle a short distance above the bed.  Now we will manually adjust this to get the height offset correct for your machine.

1. Start the print "ZOffsetAdjust" from the benchmark folder on the SDcard.
1. Go to the "live-z-adjust" setting in the menu
1. Adjust the setting until the nozzle is close to but not touching the bed.
1. Try to adjust to get the layer adhering well and quite smooth.
1. Repeat as necessary.

You can also do this adjustment on the first layer of any print to improve first layer quality.  First layer quality is the most important part of making successful prints.

Unfortunately, this offset is very sensitive to the temperature of the inductive sensor.  Therefore, you will need to make sure that similar procedure is used for each print so that the temperature of the inductive sensor is similar each time the printer measures the bed height (at the beginning of each print).

## Measure extrusion

You may need to measure if your extruder is extruding the amount of filament that it thinks it is.

  
#### [Previous Step: brain](brain.md) &nbsp;&nbsp;&nbsp; [Next Step: enjoy]
