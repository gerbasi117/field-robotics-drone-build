# UAV System Architecture

This repository documents a hands-on field robotics UAV build focused on hardware/software integration, telemetry, sensing, power distribution, and future autonomy workflows.

## System block diagram

```mermaid
flowchart TD
    A[2x 6S LiPo Battery Packs\nParallel XT90 / XT90-S] --> B[Power Module / PDB]
    B --> C[Flight Controller\nModalAI Flight Core V2]
    B --> D[4-in-1 ESC\nHolybro Tekko32 F4 65A]
    D --> E[4x EMAX ECO II Motors]
    C --> F[GPS\nModalAI u-blox M10]
    C --> G[Telemetry Radio\n915 MHz]
    C --> H[Range Sensors\nTFmini Plus]
    C --> I[LiDAR / Perception Sensor\nRP-Lidar S2]
    J[Ground Station / Laptop] <--> G
    J --> K[UAV Telemetry Ground Station Project]
```

## Integration focus

This project is not just a parts list. The purpose is to show systems integration thinking:

- power flow
- sensor layout
- telemetry plan
- safety checklist
- bring-up sequence
- failure modes
- field-test workflow
- software tooling for logs and diagnostics
