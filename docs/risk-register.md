# Risk Register

| Risk | Impact | Mitigation |
|---|---|---|
| Incorrect power wiring | Damaged electronics or battery hazard | Verify polarity, continuity, connector type, and fuse/anti-spark strategy before connecting packs. |
| ESC/motor mismatch or prop loading | High current draw, overheating, instability | Bench-test motors without props first, monitor temperature/current, and confirm prop selection. |
| GPS interference or poor placement | Poor localization or unsafe autonomous behavior | Mount GPS away from high-current wiring and RF noise, require GPS lock before GPS-dependent modes. |
| Telemetry link loss | Loss of operator situational awareness | Configure failsafe behavior and validate telemetry range/link quality before field tests. |
| Sensor vibration/noise | Bad range/IMU readings | Use secure mounting, vibration isolation where needed, and sanity-check sensor data in logs. |
| Battery sag under load | Voltage drop, brownout, unsafe flight | Monitor voltage/current, validate pack health, and set conservative battery warnings. |
| Software command without safety gate | Unsafe actuation | Keep physical commands human-controlled; route future automation through explicit safety gates. |
| Insufficient test area | Crash/property damage | Use controlled open area, pre-flight checklist, spotter, and conservative test plan. |

## Engineering note

A key goal of this project is to treat UAV bring-up like an integration process, not just a build. Every subsystem should have a bench test, integration test, and field-test validation path.
