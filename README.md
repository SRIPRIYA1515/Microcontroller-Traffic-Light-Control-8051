# Microcontroller-Traffic-Light-Control-8051
Microcontroller Traffic Light Control 8051
Our objective of this project is to simulate the traffic light system with pedestrian crossing.
In day mode, the sequence of traffic lights and pedestrian crossing signals, including green, yellow, and red lights for both traffic and pedestrians. In night mode, it is a constant blinking yellow light for traffic. 
Microcontroller Traffic Light Control (8051 Assembly code):

This assembly code is designed to control a traffic light system using an 8051 microcontroller.
It includes logic to handle both regular and pedestrian modes based on the state of a physical switch (switch1).
In pedestrian mode, it allows pedestrians to cross the road safely by controlling the traffic and pedestrian lights in a synchronized manner.
In regular mode, it simulates the typical sequence of traffic lights, transitioning between green, yellow, and red lights for traffic.
The code demonstrates the use of timer interrupts for generating accurate delays, essential for coordinating the timing of the traffic light sequence.
It showcases low-level hardware control and efficient use of the microcontroller's resources to achieve the desired functionality.


DESCRIPTION OF THE CODE:
It starts by defining the T0M1delay() function, which uses Timer 0 in mode 1 to create a delay of approximately 0.5 seconds.
The code reads the state of switch1, likely connected to a physical switch, to determine if it should operate in pedestrian mode (switch pressed) or regular mode (switch not pressed).
In pedestrian mode (switch pressed), it controls the traffic lights and pedestrian signals accordingly:
Traffic light is red, and pedestrian light is green for approximately 3 seconds.
Then traffic light turns yellow for approximately 1 second, while the pedestrian light remains red.
In regular mode (switch not pressed), it simulates the traffic light sequence:
Traffic light starts with yellow for approximately 0.5 seconds.
Then it turns green for approximately 0.5 seconds.
The cycle repeats indefinitely.
This code assumes specific hardware connections and timings. The T0M1delay() function generates accurate delays for controlling the traffic light sequence. The switch1 input determines whether the system operates in pedestrian or regular mode.
