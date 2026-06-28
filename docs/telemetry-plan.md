# Telemetry Plan

## Purpose

Telemetry is the main bridge between the UAV and the operator/debugging workflow. The goal is to monitor vehicle health, detect unsafe states, record flight logs, and support later autonomy/perception development.

## Planned telemetry fields

- Flight mode
- Armed/disarmed state
- GPS fix and satellite count
- Latitude and longitude
- Altitude
- Heading
- Battery voltage
- Battery percentage / estimated remaining energy
- Current draw
- Telemetry link quality
- IMU status
- Rangefinder readings
- Warning states

## Ground-station software

The companion project `uav-telemetry-ground-station` currently simulates telemetry and displays a live dashboard. It includes warning-state logic and flight-log recording/replay.

Future live-vehicle integration targets:

- MAVLink telemetry stream
- PX4 or ArduPilot compatibility
- Serial/USB telemetry input
- Saved flight-log import and replay
- Map view and operator checklist integration

## Warning states

Planned warning states include:

- LOW_BATTERY
- CRITICAL_BATTERY
- GPS_LOST
- LOW_SATELLITE_COUNT
- HIGH_CURRENT_DRAW
- LOW_LINK_QUALITY
- SENSOR_FAULT
- RANGEFINDER_TOO_CLOSE
- ARMED_WITH_BAD_GPS
- TELEMETRY_TIMEOUT

## Field-test workflow

1. Run pre-flight checklist.
2. Confirm telemetry link.
3. Confirm GPS status and satellite count.
4. Confirm battery voltage/current reporting.
5. Confirm rangefinder/sensor reporting.
6. Run short hover/ground tests.
7. Save telemetry logs.
8. Review warnings and anomalies after test.
