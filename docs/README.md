# Diagrams

| File | Status |
| --- | --- |
| [`block_diagram.svg`](block_diagram.svg) | Recreation of the system block diagram pasted in chat (Sensing → Processing → Control → Ladder logic → Actuation → Output). |
| [`wiring_diagram.svg`](wiring_diagram.svg) | Recreation of the wiring/interconnection diagram pasted in chat (sensors → ESP32 → PLC → relays → power). |
| [`ladder_logic_PLACEHOLDER.svg`](ladder_logic_PLACEHOLDER.svg) | Rung-overview sketch, kept as a **placeholder**. |
| `physical_setup.png` | **Not added** — no photo of the physical build was provided. |

## Important caveats

- **These are not the team's original files.** They were recreated from
  images pasted into a chat conversation, not copied from disk — this repo
  was set up from an isolated environment with no access to the local
  Downloads folder the original PNGs live in. Replace all three SVGs with
  the team's real exports/photos when available.
- **`ladder_logic_PLACEHOLDER.svg` contains template placeholder text**
  (`-abc-`, `-lmn-`, `-xyz-`, `XXXX XXXXLXXX XXX`, generic `S1`/`STOP`/`EN`
  wiring) copied faithfully from the source image — it is a rung-layout
  template, not the team's actual timer presets or ladder logic. See
  [`../plc/README.md`](../plc/README.md) for the real ladder logic status.
- No `physical_setup` photo exists in this repo yet — add one after the
  team assembles the hardware.
