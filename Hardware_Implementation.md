**PCB Functionality**
-
Attached below is the final version of our team board schematic. After receiving feedback from the teaching team in order to fix any mistakes that were made. And like mentioned earlier, the team decided to cut the humidity and IR sensor subsystems from the final project and board design. 

Final Team PCB Schematic
-
<iframe src="vertopal_53e86d8e1b304e0fba1b8ab00a47e725/media/Final_Schematic.pdf" width="100%" height="500px"></iframe>

Final Team PCB Front and Back Cadence Design
-
<iframe src="vertopal_53e86d8e1b304e0fba1b8ab00a47e725/media/PCB.pdf" width="100%" height="500px"></iframe>


Connectors
-
The first version of our PCB also contain several connectors that serve for debugging and programming purposes. Essentially, these connectors will be used to make sure that there won't be any signs of shortage, or a component drawing too much current. We wanted to focus on the data that is being sent and received from the I2C and UART ports.

Buttons
-
This version of our PCB contains 4 buttons. Three of them act as interrupts for setting the system into either the off, auto, or timer mode. Our fourth one is for resetting the ESP32.

Sensors
-
The temperature sensor is located in the center. The humidity sensor is located on the lower left hand side. And our IR subsystem is located in the lower right hand side. These three subsystems will control the motor using I2C to actuate the motor to either raise or lower the shade based on the logic it receives. 

Motor Driver
-
Located in the bottom left hand corner is our motor driver susbsystem. This subsystem will be reading the input it receives from all three sensors that were touched on previously. It will communicate through I2C.

Power and Voltage Regulator
-
Our power and voltage regulator subsystem will be located in the top left hand corner. This subsystem is responsible for receiving a wall mounted power supply of 6V and converting that to 3.3V to supply power to our other subsystems.

Version 2.0
-
If the team were to create a second version, or in this case, a third version since the final team board is version number two, our possible third board design would contain a few things. First would be doing just a little more research on surface mount components. The team ran into instances like soldering pins together when it wasn’t as visible unless it shined by a flashlight. 

Ensuring a solid 3.3V connection was another thing that could have been improved. When the team did their continuity and power check, we were able to verify that all the components on the team board were connected with a continuity check. However, when we connected our 6V power supply to the 3.3V regulator subsystem on the final board, we were unable to output that 3.3V source. So to avoid this issue, we had a separate board that contained the 3.3V subsystem that would output the necessary 3.3V source to our smaller components like the temp sensor. The reason we weren’t able to get 3.3V out of the regulator on the main board is due to the spacing between the resistors and capacitors which brings us to the next thing that would be fixed if we could make another version of the board.

Strategically placing our components on the board was the next thing that the team would have fixed if there was a chance to make another version of the board. Like mentioned before, our final version of the team board contained components that weren’t placed as strategically causing the board to not perform at the level that we had thought it would. As well as decreasing the size of the board would also be another beneficial approach that could’ve been taken upon to avoid misplacing components and not receiving the full capability of those parts.


[Back to Home](index)
