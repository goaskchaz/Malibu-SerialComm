# Malibu-SerialComm

Historical preservation and future modernization of the Malibu Hydro SerialComm SCADA system.

## Two distinct projects

| Project | Purpose | Status |
|---|---|---|
| [SerialComm Legacy](Legacy/README.md) | Preserve original VB6 v5.9, historical documents, original PIC/RTU protocol evidence | Historical / source recovery |
| [SerialComm Modern](Modern/README.md) | Raspberry Pi 5, modern HMI, CSV logs, scheduled FTP, alarm notifications and future advisory AI | Requirements / planning |

- [Modern requirements](Modern/Docs/Requirements/README.md)
- [Modern supervisory architecture](Modern/Docs/Architecture/README.md)
- [Modern hardware](Modern/Docs/Hardware/README.md)
- [Modern HMI](Modern/Docs/HMI/README.md)
- [Shared interface definitions](Shared/README.md)
- [Archive policy](Archive/README.md)

## Preservation and migration status

This is a **non-destructive first-stage organization**. Existing files under `Docs/`, `Source/`, `Config/`, `Tests/`, `Dependencies/`, `Diagrams/`, and `Releases/` are retained in place until their contents, references, and provenance can be inventoried. Legacy links point to their current paths. The historical VB6 scan text is unverified extraction, not a restored compilable project. No original PIC source or confirmed bootloader capability is yet available.

The Modernization Requirements **v0.3 PDF** was prepared separately but is **not yet uploaded to GitHub**. Its intended destination is `Modern/Docs/Requirements/SerialComm_Modernization_Requirements_v0.3.pdf`.

## Development conventions

Keep historical source evidence immutable; document corrections and reconstructions separately. Use feature branches for modern development, not separate legacy/modern branches. Proposed release tags: `legacy-v5.9` (historical identification only, not yet tagged) and `modern-v1.0.0` (future release, not yet tagged).

**Safety:** Start with offline protocol tests and read-only monitoring. Do not enable remote hydroelectric equipment commands, RTU resets, or firmware updates until original protocol support, interlocks, authorization, and field safety have been independently verified.

No license has been selected.
