# Decision Board

At some point the first robot using our CoRoSoN-Kit will be built and before that a lot of decisions have to be made. How should its individual components be designed?
Here is an overview (in keywords) of the discussed advantages and
disadvantages of the different given options.

**Important:**
This document is (of course) not complete.
It has to be further developed, depending on the state of development, in order to get finally a complete picture of the components.

**to do:**

- For each point,
  - the pros and cons are needed (in keywords).
  - a decision is needed.

## Chassis

### Size

*No decision here, every team has to decide and construct for their own.*

### Number of wheels

*No decision here, every team has to decide and construct for their own.*

## Electronic

### Logic Voltage

The logic voltage level should be 5V.
**or**
The logic voltage level should be 3.3V.

**pros:**

**cons:**

**decision:**

### Motor Voltage ([#16](https://github.com/CoRoSoN-Kit/CoRoSoN-Kit/issues/16))

The motor voltage level should be limited to 9V.
**or**
The motor voltage level should be limited to 12 V.

**pros:**

- We would be prepared should there be a rule limitation to 9 V.

**cons:**

- Rule is not there yet, may never be decided.
- Would make motor & motor driver selection more expensive & complicated.

**decision:**

We do limit to 9V, but to 12 V to be allowed in Lightweight league.

### CPU ([#18](https://github.com/CoRoSoN-Kit/CoRoSoN-Kit/issues/18))

Use of a single board chip (like Arduino Nano, Rasberry Pico, ...)
**or**
Build or own.

**pros:**

- This is the only way we can use a modern chip without soldering SMD.
- Boards are establuieshed.
- Boards are well tested.

**cons:**

- (much) more work

**decision:**

We use one (or more) single board chip(s).

We chose the [Raspberry Pi Pico](https://www.raspberrypi.com/documentation/microcontrollers/raspberry-pi-pico.html)  because it is cheap, readily available and we think it meets our requirements.

### Components ([#15](https://github.com/CoRoSoN-Kit/CoRoSoN-Kit/issues/15))

Only THT components should be used.
**or**
THT and SMD components should be used.

**pros:**

- No complicated SMD soldering for users of the kit.

**cons:**

- Significant limitation in the choice of components
- More space required

**decision:**

Only THT components should be used.
This does not mean that we do not use SMD parts at all.
If parts can be bought already soldered (e.g. an assembled motor driver board) that is of course perfectly fine.

### PCB design

There should be a minimum linewith (of ??mm) and a minimum spacing (of ??mm) between the tracks so that it is possible to etch or mill the PCB at home.

**pros:**

**cons:**

**decision:**

## Sensors

### ball

### gyroscope

### line

### distance

## Actuators

### motors

### kicker

### dribbler

## Software
