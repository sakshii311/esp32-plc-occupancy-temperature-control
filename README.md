# Automated Occupancy and Temperature Control System

Mini-project for Sensors and PLC Lab

An ESP32 reads an HC-SR501 PIR (motion) sensor and a DHT22 temperature/humidity
sensor, then drives two digital outputs into a Bosch Rexroth PLC. The PLC's
ladder logic switches a lighting relay on occupancy and a fan relay when the
measured temperature exceeds 30 °C.

## System overview

- **Sensing:** HC-SR501 PIR sensor (occupancy) + DHT22 (temperature/humidity)
- **Processing:** ESP32 reads both sensors and drives two digital outputs
  (O1 = occupancy, O2 = temperature threshold)
- **Control:** Bosch Rexroth PLC receives O1/O2 on its input module and runs
  the ladder logic program
- **Actuation:** Lighting relay (on occupancy) and fan relay (when
  temperature > 30 °C), each driving a load through relay NO/COM contacts

See [`docs/`](docs/) for the block diagram and wiring diagram, and
[`plc/`](plc/) for the ladder logic status.


