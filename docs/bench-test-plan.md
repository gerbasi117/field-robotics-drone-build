# Bench Test Plan

This plan is for staged UAV bring-up before any flight attempt.

## Stage 1: Visual and electrical inspection

- Confirm battery connectors and polarity.
- Confirm PDB/power-module wiring.
- Confirm no loose solder joints or exposed conductors.
- Confirm flight-controller mounting orientation.
- Confirm ESC signal/power connections.
- Confirm GPS and telemetry connectors.

## Stage 2: Power-up without props

- Remove all propellers.
- Power from a current-limited supply if available or use a conservative battery setup.
- Confirm flight controller boots.
- Confirm ESCs initialize.
- Confirm telemetry link connects.
- Confirm GPS is detected.
- Confirm no overheating or abnormal smell/sound.

## Stage 3: Sensor checks

- Verify GPS status and satellite count.
- Verify rangefinder readings.
- Verify IMU orientation and calibration.
- Verify telemetry data appears in ground station/logs.

## Stage 4: Motor direction test

- Props removed.
- Spin each motor individually.
- Confirm motor order and direction.
- Correct ESC/motor wiring or configuration if needed.

## Stage 5: Controlled low-power test

- Install props only after all previous checks pass.
- Use safe area and restraint procedure if appropriate.
- Validate arming behavior.
- Validate throttle response at low power.
- Monitor current, voltage, vibration, and telemetry.

## Stage 6: Initial hover test

- Open area.
- Conservative battery threshold.
- Manual control only.
- Short hover.
- Immediate post-test log review.
