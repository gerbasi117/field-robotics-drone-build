# Power Architecture

## Overview

The UAV uses two 6S LiPo battery packs in parallel to increase total capacity and current headroom. The power system is designed around safe high-current routing, voltage/current monitoring, and clean separation between propulsion power and low-current avionics/sensor power.

## Power flow

```text
CNHL 9500mAh 6S pack A
                       \
                        +--> XT90 parallel harness --> XT90-S anti-spark --> power module / PDB
                       /
CNHL 9500mAh 6S pack B

Power module / PDB
        |
        +--> ESC main input --> 4x motors
        |
        +--> regulated flight-controller power
        |
        +--> accessory/sensor power as needed
```

## Battery configuration

- Battery type: LiPo
- Pack count: 2
- Cell count: 6S each
- Nominal voltage: 22.2V each pack
- Configuration: parallel
- Purpose: increased capacity and current delivery

## Safety considerations

- Both packs must be at similar voltage before connecting in parallel.
- Anti-spark connector should be used for main connection.
- Main battery leads should be strain relieved and routed away from props.
- High-current wires should be sized appropriately and kept as short as practical.
- Low-current signal wires should be physically separated from high-current motor leads where possible.
- Power-up should happen with propellers removed during bench testing.

## Monitoring plan

The power module provides voltage/current data to the flight controller. This data will later be exposed through telemetry and monitored by the `uav-telemetry-ground-station` project for warning states such as:

- Low battery
- Critical battery
- High current draw
- Telemetry timeout
- Unsafe armed state

## Future improvements

- Add inline current verification during bench testing.
- Compare flight-controller reported voltage/current against external meter readings.
- Document connector temperatures after load testing.
- Add battery remaining estimates to telemetry dashboard.
