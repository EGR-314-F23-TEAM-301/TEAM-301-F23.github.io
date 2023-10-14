**Software Implementation**
-
Attached below is our current software diagram. Here we can see a breakdown of how our system will function in terms of the main loop, initialization, state functions, and interrupts. 

**Software State Flow Function**
-
Here we're going to break down each of the sections starting off with our main loop. Our main loop kind of holds everything together containing readings from all of our sensors and where the logic that is being analyzed from each sensor. After initializing the peripheralas and other variables, it is then transferred into an infinite loop.

In the loop, the three sensors that we choose to implement into our system loop in the following order: temperature, humidity, and light. From here, there is a state machine that will run the processing function for the current mode being used. There will be three system modes: an off, timer, and auto mode. 

Essentially the off mode will keep the system in the off position. The timer mode will leave the shade either up or down depending on the current state it's in. And once the timer reaches 0, the shade will then go in the opposite direction. Auto mode will automatically raise or lower the shade after the readings from the temperature, humidity, and light sensor go through a trial of reading the state of each sensor.

After processing the state functions, the loop will check for new inbound serial data. It can either contain a mode command, to switch to a new mode, or a timer command. Once the process has been completed, the loop starts again.

To help ensure that the system is responding, inputs given by the user are processed with an interrupt service routine that is attached in the main loop startup. When a button is pressed, the interrupt service routines call the necessary logic to change modes. 

Our last interrupt service routine will serve as a countdown to the clock in the timer mode. It sends updates to the ESP32
