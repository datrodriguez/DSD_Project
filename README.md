# DSD_Project
Drive-Through Facility Controller
A fast-food facility is developing and would like to have a digital system to help automatically
control its drive-through lane. It has a single enter/exit point (meaning at one time, there is only
one car entering or exiting). The drive-through capacity is 9 (only a maximum of 9 cars can be in
the lane at any time).
Two sensors help to indicate if there is a car at the entrance (CE) or the exit
(CX). Each sensor indicates TRUE if a car presents and FALSE otherwise. There are two traffic lights
to control if a car (at the entrance or exit) should perform its intended action (enter/leave). Each
traffic light receives digital inputs specifying whether it should be green, yellow, or red (they work
as the normal traffic lights at an intersection, red from one side, then green at the other, and
green turns yellow before turning red). There is also a seven-segment display to inform the
number of cars inside the drive-through facility.
There is a clock with a 5-second period. On each clock tick (rising edge), the lights may change
based on the traffic sensors. If there is a car wanting to leave exit light remains green, and the
counter reduces 1 every rising edge of the clock. When there is no car wanting to exit, the exit
traffic light becomes yellow for 5 seconds before turning red. Once the lane is full (9 cars inside),
the entrance traffic light turns yellow, then red after 5 seconds, and remains red if the facility is
still full. If the facility is not full, once the entrance traffic light is green, it stays green if there are
cars to enter, and the counter increases 1 every clock rising edge. Once there is no car to enter,
the entrance traffic light becomes yellow for 5 seconds before turning red.
There must also be a reset button to set the system to a known initial state (there is no car in the
facility, no car at the entrance or exit, the entrance traffic light is green by default).
