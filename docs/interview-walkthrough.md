# Interview Walkthrough: Field Robotics Drone Build

## 30-second explanation

I am building and documenting a UAV hardware/software integration project using a real flight controller, ESC, motors, batteries, GPS, telemetry radio, LiDAR/range sensors, and a planned ground-station workflow. The purpose is to show hands-on systems integration: power, wiring, sensors, telemetry, safety, bring-up, and test planning.

## What this project demonstrates

- UAV hardware integration.
- Power distribution and battery planning.
- Flight controller / ESC / motor system understanding.
- GPS, telemetry, and sensor integration planning.
- Field-test safety process.
- Documentation discipline for real robotic systems.

## How it connects to software

This build pairs with the `uav-telemetry-ground-station` project. The physical UAV is the hardware platform, and the telemetry ground station is the software tool for monitoring, logging, replaying, and reporting field-test data.

## What I would discuss in an interview

- How I selected the major components.
- How power flows through the system.
- How I would bench-test before flight.
- How I would validate telemetry and GPS health.
- How I would use logs to debug current draw, GPS loss, link issues, and sensor faults.
- How I would safely add autonomy later.
