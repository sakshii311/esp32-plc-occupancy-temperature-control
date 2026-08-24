# Firmware — pending

`occupancy_temp_control.ino` has not been added yet.

No working ESP32 sketch was available at repo-setup time, and it has not
been reconstructed or invented — the wiring/pin mapping shown in
[`../../docs/`](../../docs/) (GPIO14 ← PIR OUT, GPIO15 ← DHT DATA, two
digital outputs to the PLC input module) should be treated as a reference
for the pin layout, not as verified working firmware.

**To do:** add the real `occupancy_temp_control.ino` sketch here once it
exists, covering:

- PIR (HC-SR501) read on GPIO14
- DHT22 read on GPIO15
- Digital output O1 (occupancy) and O2 (temperature > 30 °C threshold) to
  the PLC input module
- Shared ground between ESP32 and PLC input COM
