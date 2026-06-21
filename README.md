# embedded-systems-projects
Embedded Systems projects built using Arduino on Wokwi Simulator
# Project 1 — LED Button Control 🔴

## What It Does
- Button NOT pressed → LED OFF
- Button pressed → LED ON solid
- Button held > 1 second → LED blinks fast
- Button released → LED OFF

## Circuit
| Component | Pin |
|---|---|
| LED + 220Ω resistor | Pin 13 |
| Push Button + 10KΩ pull-down | Pin 2 |

## Concepts Learned
- GPIO Input and Output
- Pull-down resistor (prevents floating pin)
- Boolean flag variables (state management)
- Non-blocking timer using millis()
- Serial communication (UART)

## Key Code Concepts
```c
// Non-blocking timer
if (millis() - pressStartTime >= 1000) {
    // held for 1 second!
}

// Boolean flag
bool isPressed = false;  // tracks button state
```

## Simulate It
Open in Wokwi → Press ▶ Play → Click and hold button!

## What I Learned
How to read digital inputs, manage states with 
flags, and use non-blocking timers instead of delay()
