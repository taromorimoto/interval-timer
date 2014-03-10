interval-timer
==============

A simple interval timer for Arduino.

Example usage:

```
#include "IntervalTimer.h"

void setup() {
  Serial.begin(9600);
}

void myFunctionA() {
	Serial.println("Hello A!");
}

void myFunctionB() {
	Serial.println("Hello B!");
}

IntervalTimer timerA(1000, myFunctionA);
IntervalTimer timerB(3000, myFunctionB);

void loop() {
	timerA.update();
	timerB.update();
}
```

You can just make a zip of the IntervalTimer folder and add as a library in Arduino IDE.
