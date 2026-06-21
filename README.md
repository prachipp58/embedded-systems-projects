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

## 🔗 Live Simulation
[▶ Run on Wokwi](https://wokwi.com/projects/467442347721820161)

# Project 3 — Temperature Monitor 🌡️

## What It Does
| Temperature | LED | Buzzer | LCD Status |
|---|---|---|---|
| Below 40°C | OFF ⚫ | Silent | Status: Normal |
| Above 40°C | ON 🔴 | Silent | WARNING! Hot! |
| Above 50°C | ON 🔴 | Beeping 🔊 | !! DANGER !! |

## Circuit Connections
| Component | Connection |
|---|---|
| Potentiometer SIG | Pin A0 |
| Potentiometer VCC | 5V |
| Potentiometer GND | GND |
| LCD SDA | Pin A4 |
| LCD SCL | Pin A5 |
| LCD VCC | 5V |
| LCD GND | GND |
| LED + 220Ω | Pin 9 |
| Buzzer | Pin 8 |

## Concepts Learned
- ADC (Analog to Digital Conversion)
- I2C Protocol (LCD communication)
- Threshold based alert logic
- Real time monitoring with millis()
- UART Serial data logging
- Sensor simulation with potentiometer

## How to Test
Turn pot LEFT →  temperature goes DOWN 

Turn pot RIGHT → temperature goes UP

Test 1: Pot at 25% → Temp: 25°C | Normal

Test 2: Pot at 45% → Temp: 45°C | WARNING + LED ON

Test 3: Pot at 55% → Temp: 55°C | DANGER + Buzzer!

## 🔗 Live Simulation
[▶ Run on Wokwi](https://wokwi.com/projects/467443390009625601)
