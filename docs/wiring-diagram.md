# Wiring Diagram

## High-level wiring plan

```text
[Battery A] --\
              +--> [XT90 Parallel Harness] --> [XT90-S Anti-Spark] --> [Power Module / PDB]
[Battery B] --/                                                        |
                                                                       +--> [4-in-1 ESC]
                                                                       |       |--> Motor 1
                                                                       |       |--> Motor 2
                                                                       |       |--> Motor 3
                                                                       |       |--> Motor 4
                                                                       |
                                                                       +--> [Flight Core V2]
                                                                                |--> GPS
                                                                                |--> Telemetry radio
                                                                                |--> Receiver
                                                                                |--> Range sensors
                                                                                |--> Future perception sensors
```

## Wiring principles

- Keep battery and ESC power leads short and mechanically secure.
- Route signal wires away from motor/ESC power wiring where possible.
- Use strain relief on connectors attached to the flight controller.
- Label connectors before final assembly.
- Bench-test one subsystem at a time.
- Remove propellers for all bench power-up and configuration tests.

## Signal wiring notes

- Flight controller telemetry ports should use the correct JST connector type and pinout.
- Sensor wiring should be verified with pinout documentation before applying power.
- Range sensors and telemetry radios should be powered only from appropriate regulated outputs.
- Receiver and telemetry antennas should be mounted with clear separation from noisy power wiring.

## To be added

- Final pinout table
- Photos of each subsystem
- Continuity-check results
- Sensor mounting layout
