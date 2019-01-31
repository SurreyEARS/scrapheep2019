## Getting Started

Install the latest Arduino IDE (1.8.8), Available for most OS's. Open it up. 

`Tools -> Manage Libraries (Click)`

Search Box: `adafruit l293`

Install `Motor Driver Library by CuriosityGym`

An example is provided by the library in:
  `File -> Examples -> Motor Driver Library -> basicDriver`


## Coding Hints
`MotorDriver m; // Required at the top of every sketch using the motor driver library`

### This allows you to use the functions:

 ` m.motor(MOTOR NUMBER [1-4], MODE [FORWARD|BACKWARD|BRAKE|RELEASE], SPEED [0-255]); 
//Drives the selected MOTOR NUMBER in the given MODE, at the given SPEED`


`m.motor_output (MOTORx_A/B, HIGH|LOW, SPEED [0-255]); // Allows you to drive solenoids and lights, directly writes to the driver. `

For more information on the functions, and the code behind them check out this repo:
  https://github.com/CuriosityGym/MotorDriver

The documentation of the functions available is here as part of the source code:
  https://github.com/CuriosityGym/MotorDriver/blob/master/src/MotorDriver.cpp



Arduino is a superset of C, but a subset of C++. 

The function "setup" runs once at power up, and every time the Uno is hardware-reset. 
The "loop" function runs continuously until the end of time. 

Check out the Arduino Code Reference: https://www.arduino.cc/reference/en/

***


### When its time to test your code
Connect your Arduino Uno then follow:

  `Tools -> Board: "xxxxxxxxxxx" -> Arduino/Genuino Uno`

  `Tools -> Port: "xxxxxxx" -> Whichever COM port appears when the Uno is connected`

  `Sketch -> Upload`

***

Test Compiles without uploading, nor having the board connected can be done using:
  `Sketch -> Verify/Compile`