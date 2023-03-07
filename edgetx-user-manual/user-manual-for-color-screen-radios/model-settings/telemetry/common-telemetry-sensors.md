# Vanliga telemetrisensorer

Följande sensorer är vanligt förekommande och detekteras normalt sett automatiskt av EdgeTX:

| Namn | Beskrivning                              | Datakälla             |
| ---- | ---------------------------------------- | --------------------- |
| 1RSS | Mottagen signalstyrka antenn 1 (RSSI)    | Mottagare             |
| 2RSS | Mottagen signalstyrka antenn 2 (RSSI)    | Mottagare             |
| Rqly | Mottagarens länkkvalitet (giltiga paket) | Mottagare             |
| RSNR | Mottagarens signal/brusförhållande       | Mottagare             |
| RFMD | Receiver packet rate                     | Mottagare             |
| TPWR | Sändarens sändareffekt                   | Sändare               |
| TRSS | Sändarens signalstyrka antenn            | Sändare               |
| TQly | Sändarens länkkvalitet (giltiga paket)   | Sändare               |
| TSNR | Sändarens signal/brusförhållande         | Sändare               |
| ANT  | Sensor endast för debugging              | Sändare               |
| GPS  | GPS-koordinater                          | GPS / Styrkort        |
| Alt  | GPS-höjd                                 | GPS / Styrkort        |
| Sats | Antal uppkopplade satelliter             | GPS / Styrkort        |
| Hdg  | Magnetisk orientering                    | GPS / Styrkort        |
| RXBt | Batterispänning                          | Styrkort              |
| Curr | Strömförbrukning                         | Styrkort              |
| Capa | Återstående batterikapacitet             | Styrkort              |
| Ptch | FC Pitch angle                           | Styrkort              |
| Roll | FC Roll angle                            | Styrkort              |
| Yaw  | FC Yaw angle                             | Styrkort              |
| FM   | Flygläge                                 | Styrkort              |
| VSPD | Vertikal hastighet                       | Styrkort m. barometer |
