# Diagrams

| File | Status |
| --- | --- |
| [`block_diagram.png`](block_diagram.png) | System block diagram (Sensing → Processing → Control → Ladder logic → Actuation → Output). |
| [`wiring_diagram.png`](wiring_diagram.png) | Wiring/interconnection diagram (sensors → ESP32 → PLC → relays → power). |
| [`ladder_logic_PLACEHOLDER.png`](ladder_logic_PLACEHOLDER.png) | Rung-overview sketch, kept as a **placeholder**. |
| `physical_setup.png` | **Not added** — no photo of the physical build was provided. |

## Important caveats

- **`ladder_logic_PLACEHOLDER.png` contains template placeholder text**
  (`-abc-`, `-lmn-`, `-xyz-`, `XXXX XXXXLXXX XXX`, generic `S1`/`STOP`/`EN`
  wiring) — it is a rung-layout template, not the team's actual timer
  presets or ladder logic. See [`../plc/README.md`](../plc/README.md) for
  the real ladder logic status. Replace this file with a real IndraLogic
  export once available, and drop the `_PLACEHOLDER` suffix.
- No `physical_setup` photo exists in this repo yet — add one after the
  team assembles the hardware.
