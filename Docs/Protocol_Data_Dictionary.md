# Protocol and Data Dictionary — Historical Baseline

Source: scanned SerialCom technical report (41-page PDF), especially scan pages 7–14 and 34–37.

## Data burst
The report defines an RTU indicator `@AAA`, three-character sensor tags, values and a terminating line ending. The printed examples and delimiters are not fully consistent. **Do not implement an operational parser without verifying the original scans and source.**

## Commands
The report describes `?` request, RTU identifier, plus/minus action and expected `!` response. Appendix C lists controls for cameras, lighting, valves, fans and startup/shutdown. These are historical descriptions, not instructions to operate equipment.

## Files
- `set.ini`: port, baud, data bits, stop bits, parity, flow
- `CMD.dat`: command definitions
- `DPL.dat`: sensor labels and critical values
- `rtu_download.txt`: last captured burst
- `ftp_upload.txt`: prepared upload data
- `RTU.log`, `Sys.log`: planned logging

## Selected labels from Appendix B
`dwl` Water Level; `dhl` Header Level; `dfd` Filter Differential; `dby` Battery Voltage; `dat` Air Temperature; `dwt` Water Temperature; `def` Excess Over Flow.

## Unresolved
RTU names `BPH`, `BIG`, `PWR`; burst separator, numeric width, CR/LF ordering, acknowledgment behavior and alarm comparison semantics require source verification.
