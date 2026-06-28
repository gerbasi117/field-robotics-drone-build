# Power Architecture

## Goal

Document the high-current power path and low-voltage electronics path before flight testing.

## Power path

```text
2x 6S Batteries in Parallel
   -> XT90-S Anti-Spark / Parallel Harness
   -> Power Module / PDB
   -> ESC 4-in-1
   -> Motors
```

## Electronics path

```text
Power Module / Regulated Output
   -> Flight Controller
   -> GPS / telemetry / receiver / sensors as allowed by power budget
```

## Safety notes

- Verify polarity before connecting electronics.
- Use a smoke stopper/current limiter for first power-on when possible.
- Confirm ESC capacitor installation and secure mounting.
- Keep props removed during bench testing.
- Verify battery voltage before connecting.
- Check connector heat after bench runs.
- Log voltage sag/current draw during staged tests.

## Open questions

- Final connector path?
- Final current rating of each connector/wire segment?
- Sensor power source?
- Total electronics current draw?
- ESC current draw during hover estimate?
