# System Overview

## Purpose

This project documents a custom UAV platform intended for field-robotics experimentation, telemetry monitoring, sensor integration, and future autonomy/perception workflows.

The build is intentionally treated like a small robotics integration project instead of only a hobby drone. The focus is on repeatable documentation, safe power-system design, clean wiring, sensor/telemetry planning, and structured testing.

## High-level architecture

```text
2x 6S LiPo packs in parallel
        |
        v
XT90 parallel harness / anti-spark connector
        |
        v
Power module / power distribution
        |
        +--> ESC power input --> 4x brushless motors
        |
        +--> Flight controller regulated power
                    |
                    +--> GPS
                    +--> Telemetry radio
                    +--> Range sensors / future perception sensors
                    +--> Receiver / control link
```

## Primary objectives

1. Build a reliable multirotor hardware platform.
2. Document power, wiring, and safety decisions.
3. Add telemetry and sensor workflows that support debugging and field tests.
4. Build software tools around telemetry, warning states, and operator support.
5. Use the platform as a long-term base for robotics/autonomy projects.

## Future software integration

This physical build is paired with the `uav-telemetry-ground-station` project. That software project currently uses simulated telemetry and will later support MAVLink/PX4/ArduPilot-style integration for live vehicle monitoring, logging, and warning-state detection.
