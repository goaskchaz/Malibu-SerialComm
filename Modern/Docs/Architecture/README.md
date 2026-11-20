# Proposed Supervisory Architecture

```text
PWR PIC RTU ----\\
DAM PIC RTU -----+-- existing radio network -- radio modem -- isolated RS-232 -- Raspberry Pi 5
MLK PIC RTU ----/                                                      |          |
                                                                      |          +-- SSD / CSV archive
                                                                      +-- Local HMI / alarm engine
                                                                                  |
                                                                          Firewall / Internet
                                                                                  |
                                                                       Existing offsite FTP site
```

The Raspberry Pi hosts independent serial collector, protocol decoder, logger, alarm evaluator, scheduler/uploader, and browser HMI services. Future advisory AI reads historical data and raises recommendations, never direct actuation. Future email/text-to-speech radio alerts require a separate authorized communications gateway; do not assume the existing telemetry radio channel supports voice.

**Safety:** initially read-only; commands require independently verified protocol, operator authorization, interlocks and offline tests. External network traffic must not directly access the RTU control channel.
