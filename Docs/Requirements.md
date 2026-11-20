# SerialComm Requirements — Proposed

The following are proposed, not verified implementation features.

| ID | Requirement |
|---|---|
| SC-FR-001 | Configure serial link parameters. |
| SC-FR-002 | Open and close a serial connection and report status. |
| SC-FR-003 | Buffer partial incoming messages. |
| SC-FR-004 | Validate message framing and integrity using the verified protocol. |
| SC-FR-005 | Identify RTU source and timestamp received messages. |
| SC-FR-006 | Decode documented telemetry fields. |
| SC-FR-007 | Log communication faults and recoverable errors. |
| SC-FR-008 | Provide data logging and HMI integration. |
| SC-FR-009 | Separate read-only monitoring from control actions. |
| SC-FR-010 | Reject invalid or unauthorized commands. |
| SC-FR-011 | Support offline test data or replay. |
| SC-FR-012 | Fail safely on communications loss. |

## Open questions
Original project boundaries, COM/ActiveX controls, modem type, baud/parity, flow control, RTU addressing, packet framing, checksums, retries and supported commands require verification.
