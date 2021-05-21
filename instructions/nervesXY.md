# McP Assembly Instructions

## Nerves

Generally, you will be making wires with JST connectors on the ends.  Each JST connector has a small indicator cutout nearer one end.  We will call the pin on that end one, and the rest two, three, et cetera.  

Our JST connectors for the motors will have blue, red, green, and black wires.  For the 4 pin JST XH ends: black=1, green=2, blue=3, red=4.  However, for the 6 pin JST PH ends: black=1, blue=3, green=4, red=6, and pins 2 and 5 are not connected.

### X&Y motor cables
 


#### Parts  

* 1x 1000mm 4 wire cable with 6 pin JST PH connector and 4 pin JST XH connector
* 1x 4 pin JST XH connector
* 4x JST XH pins
* 1x 6 pin JST PH connector
* 4x JST PH pins
* JST crimping tool

#### Assembly

1. Turn the 1000mm cable into two identical 500mm cables each with a 6 pin JST PH connector and a 4 pin JST XH connector.  Ask for help if needed.
1. Cut the cable in half.
1. Strip off about 2mm of insulation on each of the 8 newly created ends.
1. Take the cable with the 6 pin JST PH on one end.  On each of the newly stripped ends, crimp a JST XH pin (the larger of the two pin sizes).
1. Insert these newly crimped pins into the 4 pin JST XH connector: black=1, green=2, blue=3, red=4.
1. Take the cable with the 4 pin JST XH on one end.  On each of the newly stripped ends, crimp a JST PH pin (the smaller of the two pin sizes).
1. Insert these newly crimped pins into the 6 pin JST PH connector: black=1, blue=3, green=4, red=6, and pins 2 and 5 are not connected.
1. Verify that your two cables are identical: 4 pin XH to 6 pin PH, with blue and green wires twisted.  One will be attached to your x-motor, the other to your y-motor.


#### [Previous Step: nerves](nerves.md) &nbsp;&nbsp;&nbsp; [Next Step: nervesZ](nervesZ.md)


