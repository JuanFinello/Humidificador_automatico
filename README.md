# Automatic humidifier (Arduino)

Arduino sketch that keeps a room at a humidity setpoint. Firmware based on AlexGyver's
design.

## How it works

A DHT22 sensor reads relative humidity and a potentiometer sets the target. When the
reading falls below the target, the sketch switches the humidifier on through a MOSFET and
off again once the target is reached. Two LEDs show the state.

| Pin | Use |
|---|---|
| A1 | Setpoint potentiometer |
| 2 | MOSFET driving the humidifier |
| 3, 4, 5 | DHT22 power, data and ground |
| 11, 12 | Status LEDs |

## Stack

Arduino (C++) · DHT22
