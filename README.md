# sinusoidal
It is a sample project to show how to calculate the timing for a stepper motor with a sinusoidal s-curve.

There is some code for ESP32 and some other for Arduino UNO. While my idea is to do the required calculations in real-time, the limited RAM and computing power of the UNO is not a problem if the delays are pre-calculated on an array. Of course that may not work for movements that require more than 400 steps for acceleration phase, so this is just a demo. 

You will find in accel_shapes_uno four different speed profiles: linear, a cubic s-curve, a exponential one (whith high-acceleration at low speeds only) and a sinusoidal s-curve. You can see a [video](https://www.youtube.com/watch?v=dbEqo6J-ruA) of it in action (it changes the direction each cycle of the four patterns).
