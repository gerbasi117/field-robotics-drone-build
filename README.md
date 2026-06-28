# Field Robotics Drone Build

UAV hardware/software integration documentation for a custom multirotor platform built as a field-robotics portfolio project.

This repo documents the vehicle architecture, component selection, power system, wiring plan, telemetry plan, pre-flight safety process, and integration-test workflow for a custom UAV platform. The goal is to demonstrate practical UAV/robotics systems integration skills: flight controller setup, ESC/motor wiring, battery/power planning, telemetry, sensors, safety checks, and field-test planning.

## Target roles this project supports

- Systems Integration Engineer - UAV/Robotics
- UAV Integration Engineer
- Robotics Integration Engineer
- Field Robotics Engineer
- Robotics Test Engineer
- Mission Operations Engineer
- Technical Operations Engineer - Robotics

## Current status

- Hardware selected and being assembled
- Wiring/power architecture planned
- Telemetry and sensor integration planned
- Photos and field-test notes will be added as build progresses

## Main subsystems

- Flight controller: ModalAI Flight Core V2
- ESC: Holybro Tekko32 F4 Metal 4-in-1 65A, 6S
- Motors: EMAX ECO II 2207 1700KV x4
- Props: HQProp DP 7x3.5x3 tri-blade
- Batteries: 2x CNHL 9500mAh 6S packs in parallel
- GPS: ModalAI u-blox M10
- Telemetry: 915MHz telemetry pair
- Sensors: RP-Lidar S2, TFmini Plus rangefinders, FLIR Lepton/PureThermal 3
- Camera: GoPro Hero 13 for recording; FPV system planned for live feed

## Documentation

- [System Overview](docs/system-overview.md)
- [Parts List](docs/parts-list.md)
- [Power Architecture](docs/power-architecture.md)
- [Wiring Diagram](docs/wiring-diagram.md)
- [Telemetry Plan](docs/telemetry-plan.md)
- [Safety Checklist](docs/safety-checklist.md)
- [Integration Test Plan](docs/integration-test-plan.md)

## Resume bullets

- Designed and documented a UAV hardware/software integration project involving flight controller, ESCs, motors, GPS, telemetry radios, LiDAR/range sensors, high-current batteries, power distribution, and field-test planning.
- Created system documentation including wiring layout, power architecture, component selection, safety checklist, and integration-test plan.
- Planned telemetry and perception integration workflows for field testing, diagnostics, and future autonomous behavior.
