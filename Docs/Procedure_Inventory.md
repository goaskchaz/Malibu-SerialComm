# VB6 Procedure Inventory — Historical Baseline

Source: scan pages 21–29 and 38–41. Names below may represent multiple revisions.

| Name | Documented role |
|---|---|
| `MSComm1_OnComm` | Receive serial input and accumulate buffer |
| `ParseDP` | Parse data burst into readings |
| `GetRTU` | Identify remote terminal unit |
| `GetDP` | Extract sensor value |
| `SetState`, `GetState` | Evaluate and display alarm status |
| `DataPoint` | Prototype parsing routine in appended code |
| `GetCommSettings`, `GetSet` | Load and parse INI settings |
| `btnSendStart_Click` | Transmit entered command |
| `btnQuit_Click` | Close serial port and forms |
| `Form_Load` | Initialize paths, icons, settings and status |
| `btnRecStart_Click`, `btnRecStop_Click` | Open/close port |

Original form references include `frmTerminal`, `frmMon`, `frmComSet`, `frmRTUSelect`, plus differently named forms in the narrative. Confirm against actual `.frm` files before coding.
