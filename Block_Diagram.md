**Block Diagram**
-
The block diagram helps visualize and understand the functionality of each individual subsystem and their respective components work and align together with the micro-controller.

**Current Block Diagram**
-

<iframe src="vertopal_53e86d8e1b304e0fba1b8ab00a47e725/media/blockdiagram.pdf" width="100%" height="500px"></iframe>

**Individual Subsystems**
-
Each individual can be found in the Block Diagram within the dashed boxes that contains a member's name highlighted in yellow.

**Microcontroller and Power Regulator**
-
The **PIC24FJ64GA702** microcontroller selected for this project has all of the I2C, GPIO, UART, ESP32, ICSP, and WIFI pins to run the final design. The selected voltage regulator MIC4575WU satisfies the requirements of operating at a 3.3V range by using a switching voltage regulator that provides the voltage to the serial sensors that are implemented.

**Temperature Sensor**
-
The project requires at least two different environmental conditions through at least two separate serial sensors. The **TC74** temperature sensor subsystem will sense at least one of the conditions.

**Humidity Sensor**
-
Measuring humidity is another environmental factor that the project requires and the **HIH6030-021-001** humidity sensor will sense the second required environment condition.

**Light Sensor**
-
Due to having an extra group member added to the team, the team had to come up with another subsystem to divide the work evenly amongst the group. So the team decided on adding a light sensor subsystem **LM358DGKR**

**Motor Driver and Motors**
-
The project requires at least one motor/serial actuator to be controlled by a motor controller that will communicate over SPI or I2C-based protocol.

[Back to Home](index)
