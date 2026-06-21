# embedded-systems-projects
Embedded Systems projects built using Arduino on Wokwi Simulator

# Project 1 — LED Button Control 🔴

## What It Does
| Action | Result |
|---|---|
| Button NOT pressed | LED OFF |
| Button pressed | LED ON solid |
| Button held > 1 second | LED blinks fast |
| Button released | LED OFF |

## Circuit Connections
| Component | Connection |
|---|---|
| LED Anode (+) | 220Ω → Pin 13 |
| LED Cathode (-) | GND |
| Button Pin 1 | Pin 2 |
| Button Pin 2 | 5V |
| Button Pin 1 | 10KΩ → GND (pull-down) |

## Concepts Learned
- GPIO Input and Output
- Pull-down resistor (prevents floating pin)
- Boolean flag variables (state management)
- Non-blocking timer using millis()
- Serial UART communication

## Serial Monitor Output
## 🔗 Live Simulation
[▶ Run on Wokwi](paste your wokwi link here)
