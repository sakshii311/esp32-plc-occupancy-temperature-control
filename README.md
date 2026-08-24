# Automated Occupancy and Temperature Control System

Mini-project for **MTE 2243 — Sensors and PLC Lab**, [DEPARTMENT NAME], Manipal Institute of Technology.

An ESP32 reads an HC-SR501 PIR (motion) sensor and a DHT22 temperature/humidity
sensor, then drives two digital outputs into a Bosch Rexroth PLC. The PLC's
ladder logic switches a lighting relay on occupancy and a fan relay when the
measured temperature exceeds 30 °C.

## Team

5-person team, [TEAM NAME / SECTION].

| Role | Name |
| --- | --- |
| Repo owner | [YOUR NAME] |
| Firmware | [TEAM MEMBER] |
| PLC / ladder logic | [TEAM MEMBER] |
| Wiring / hardware | [TEAM MEMBER] |
| Documentation | [TEAM MEMBER] |

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

## Repository structure

```
.
├── firmware/
│   └── occupancy_temp_control/   # ESP32 sketch (Arduino)
├── plc/                          # Bosch Rexroth / IndraLogic project files
├── docs/                         # Block diagram, wiring diagram, ladder logic
└── README.md
```

## Status

- [ ] ESP32 firmware — not yet added, see [`firmware/occupancy_temp_control/README.md`](firmware/occupancy_temp_control/README.md)
- [ ] PLC / IndraLogic project files — pending next lab session, see [`plc/README.md`](plc/README.md)
- [ ] Ladder logic diagram — currently a template placeholder, see [`docs/README.md`](docs/README.md)
- [ ] Physical setup photo — not yet added

## License

[LICENSE — e.g. MIT, or "coursework, not licensed for reuse"]
