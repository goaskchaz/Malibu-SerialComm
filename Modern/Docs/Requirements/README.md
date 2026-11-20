# Modern SerialComm Requirements

**Document baseline:** SerialComm Modernization Requirements v0.3 (PDF prepared separately; binary not yet committed to GitHub).

The requested PDF belongs at `Modern/Docs/Requirements/SerialComm_Modernization_Requirements_v0.3.pdf` once uploaded with a binary-capable Git workflow. Do not treat this link as an existing repository file.

## Requirement domains
1. Raspberry Pi 5, SSD, UPS, isolated RS-232 and low-cost industrial accessories.
2. Three existing PIC RTUs and radio-modem protocol preservation.
3. Modern browser HMI with level cylinders, trends, alarm status, and RX/TX console.
4. Timestamped incoming/outgoing burst capture and CSV retrieval by date/RTU/direction; separate sensor, alarm, system, and FTP logs.
5. Configurable scheduled offsite file transfers with retries and audit trail. Server address/credentials are pending.
6. Future AI monitoring (advisory only) and threshold-based email/text-to-speech radio notifications subject to safety and regulatory review.
7. Remote PIC sensor-range/reset command generation only where original firmware/protocol supports it; remote firmware updating is a separate future feasibility item.

Historical behavior and new requirements must remain explicitly differentiated. See [legacy evidence](../../../Legacy/README.md).
