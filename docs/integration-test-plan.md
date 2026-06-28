# Integration Test Plan

## Goal

Safely bring up the UAV one subsystem at a time and document results. This test plan is designed to reduce risk and create a repeatable workflow for hardware/software integration.

## Phase 1: Static hardware inspection

- Verify frame integrity.
- Verify battery bay and mounting hardware.
- Verify motor mounting and screw lengths.
- Verify ESC placement and airflow.
- Verify wiring strain relief.
- Verify connector orientation and polarity.

## Phase 2: Power-system bench test

- Remove all propellers.
- Connect one battery path at a time if possible.
- Confirm no unexpected heat, smoke, arcing, or voltage drop.
- Confirm flight-controller power is stable.
- Confirm voltage/current values are reasonable.

## Phase 3: Flight controller bring-up

- Connect to ground-control/configuration software.
- Verify board orientation.
- Verify sensor calibration.
- Verify GPS detection.
- Verify receiver input.
- Verify telemetry radio connection.
- Verify arming checks and failsafe settings.

## Phase 4: Motor/ESC validation

- Props removed.
- Verify motor order.
- Verify motor direction.
- Verify ESC response.
- Verify no abnormal vibration/noise.
- Verify current draw remains reasonable during low-throttle tests.

## Phase 5: Telemetry validation

- Confirm telemetry stream is received.
- Confirm GPS, altitude, battery, current, mode, armed state, and rangefinder fields.
- Save a sample telemetry log.
- Replay sample log through the `uav-telemetry-ground-station` project.

## Phase 6: Controlled field testing

- Short low-altitude hover test.
- Confirm stability and control response.
- Log telemetry.
- Review warnings/anomalies.
- Make one change at a time between test flights.

## Exit criteria for first successful integration pass

- Vehicle powers on safely.
- Flight controller, GPS, receiver, and telemetry are detected.
- Motor order/direction verified with props removed.
- Telemetry logs can be recorded and reviewed.
- Safety checklist is complete before first flight.
