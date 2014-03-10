interval-timer
==============

A simple interval timer for Arduino.

Example usage:

```
#include "IntervalTimer.h"

void setup() {
  Serial.begin(9600);
}

void myFunction() {
	Serial.println("Hello!");
}

IntervalTimer timer(1000, myFunction);

void loop() {
	timer.update();
}
```

You can just make a zip of the IntervalTimer folder and add as a library in Arduino IDE.
