# SerialComm Modern — Raspberry Pi 5 Upgrade

**Status:** planning / requirements; software release target `modern-v1.0.0` (not released).

## Scope
- Raspberry Pi 5 with SSD, UPS, electrically isolated RS-232 interface to the existing radio modem
- Preserve the three PIC-based RTUs (PWR, DAM, MLK) and radio network pending validation
- Browser HMI with telemetry, cylindrical fill-level graphics, alarms, RX/TX console and history
- Timestamped, lossless RX/TX archives and retrievable CSV logs
- Configurable scheduled FTP-compatible uploads, retry queue and transfer audit
- Authorized, verified RTU configuration commands for supported sensor ranges/resets only after protocol and firmware confirmation
- Future advisory AI anomaly detection, email notifications, and separately engineered text-to-speech radio announcements

## Requirements
- [Modern requirements index](Docs/Requirements/README.md)
- [Architecture](Docs/Architecture/README.md)
- [HMI](Docs/HMI/README.md)
- [Hardware](Docs/Hardware/README.md)

## Implementation approach
Phase 1: offline protocol replay and read-only monitoring. Phase 2: logging, HMI, alarms, scheduled uploads. Phase 3: verified operator-authorized configuration actions. Phase 4: optional AI and notifications. No automatic AI control of hydro equipment.

Existing top-level `Docs/`, `Source/`, `Config/`, `Tests/` and `Diagrams/` remain in place until their ownership is inventoried.
