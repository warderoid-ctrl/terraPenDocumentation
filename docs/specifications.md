# Specifications

| | |
|---|---|
| **Drawing area** | A2 — 594 × 420 mm |
| **Overall size** | 800 × 600 × 110 mm |
| **Weight** | Approximately 10 kg |
| **Motion** | coreXY |
| **Toolhead** | Stepper pen lift, roughly 14 mm of Z travel |
| **Controller** | ESP32 based — [ESP32 Plotter Controller](hardware.md) |
| **Firmware** | [FluidNC](YAMLConfigurationSettings.md) |
| **Power supply** | 110–240 V switching adaptor with multi-region plugs, 12 V output |
| **Connectivity** | Wi-Fi (own access point or your network), USB-C |
| **Storage** | MicroSD card, supplied and pre-loaded |
| **Input files** | SVG, PDF and G-code via [terraForge](terraForge.md); the machine plots G-code |

## Bench space

The machine is 800 × 600 mm, so allow a little more than that. Leave room at the
**rear right** to reach the power switch, and enough clearance at the front to lift
the machine when you need to reach the power inlet underneath.

Paper larger than the drawing area will overhang the machine, which is fine — but
[the artwork itself must fit](plotting.md), or the plot will crash.

!!! note "Earlier machines"
    Machines with a [solenoid pen lift](solenoid.md) differ in the toolhead only.
