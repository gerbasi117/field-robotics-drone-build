# Integration Test Plan

## Stage 1 — Documentation and inspection

- Confirm parts list.
- Photograph layout.
- Confirm wiring path.
- Confirm power architecture.

## Stage 2 — Power-on bench test

- Props removed.
- Power electronics using current-limited/safe procedure if available.
- Confirm flight controller boots.
- Confirm receiver/GPS/telemetry detected.

## Stage 3 — Motor test

- Props removed.
- Confirm motor order.
- Confirm motor direction.
- Check ESC temperature and connector heat.

## Stage 4 — Sensor test

- Confirm GPS lock.
- Confirm rangefinder data.
- Confirm telemetry messages.
- Save sample log.

## Stage 5 — Tethered / restrained test

- Verify thrust response at low power.
- Monitor current draw and voltage sag.
- Stop at any abnormal vibration, heat, or telemetry fault.

## Stage 6 — First hover

- Short low-altitude hover.
- Log telemetry.
- Inspect hardware after landing.
- Review voltage/current/GPS/IMU logs.

## Issues log

| Date | Test | Issue | Suspected Cause | Fix | Retest Result |
|---|---|---|---|---|---|
| TODO | TODO | TODO | TODO | TODO | TODO |
