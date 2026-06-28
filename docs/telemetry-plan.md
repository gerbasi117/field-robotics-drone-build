# Telemetry Plan

## Goal

Create a workflow for monitoring vehicle health, logging flight data, and diagnosing issues during bench tests and flight tests.

## Telemetry fields to monitor

- Flight mode
- Armed/disarmed state
- GPS fix
- Satellite count
- Latitude / longitude
- Altitude
- Heading
- Battery voltage
- Battery percentage
- Current draw
- Telemetry link quality
- Rangefinder distance
- IMU status
- Warning state

## Warning states

- Low battery
- Critical battery
- GPS lost
- Low satellite count
- High current draw
- Telemetry timeout
- Unsafe armed state
- Rangefinder too close
- Sensor fault

## Software link

The companion project is `uav-telemetry-ground-station`.
