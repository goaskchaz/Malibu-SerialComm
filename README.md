# Malibu-SerialComm

Legacy Visual Basic 6.0 project associated with the Malibu Hydro SCADA system.

The repository is being organized for preservation of original source, documented maintenance, and offline testing. The original SerialComm implementation has not yet been inspected. Do not assume proposed requirements are implemented.

## Structure
- `Docs/`: application description, requirements, architecture, communications, hardware, installation and change log
- `Source/Original/`: untouched recovered VB6 files
- `Source/Development/`: maintained forms, modules, classes, controls and resources
- `Config/`: sanitized examples
- `Tests/`: offline serial, protocol and RTU tests
- `Dependencies/`: OCX/DLL inventory (not proprietary binaries)
- `Diagrams/`: architecture and wiring
- `Releases/`: build and release documentation

## Next steps
Recover original `.vbp`, `.frm`, `.frx`, `.bas`, `.cls`, and `.res` files. Inventory dependencies, confirm serial protocol and test only in isolated environments before considering live equipment.

No license has been selected.

## Historical source

- [Malibu Hydro SCADA historical narrative](Docs/Historical/Malibu_Hydro_SCADA_Historical_Document.md) — original system description, HMI, radio telemetry, RTUs and load management. The source refers to figures not supplied in the text extract.
