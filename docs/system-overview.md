# System Overview

## Goal

Build and document a field robotics UAV platform that can be used for telemetry experiments, sensor integration, AI operator workflows, and future autonomy development.

## High-level architecture

```text
Battery System
   |
Power Module / PDB
   |---------------- ESCs -> Motors
   |
Flight Controller
   |---------------- GPS
   |---------------- Telemetry Radio
   |---------------- RC Receiver
   |---------------- Range Sensors / LiDAR
   |
Ground Station / Telemetry Dashboard
```

## Engineering focus

- Hardware/software integration
- Power distribution and battery safety
- Flight controller configuration
- Telemetry and log analysis
- Sensor integration
- Test planning and staged validation

## Planned software integration

- UAV telemetry dashboard
- Flight-log replay
- Warning-state detection
- Future MAVLink/PX4/ArduPilot integration
- Future AI operator assistant integration
