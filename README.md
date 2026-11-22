# Coilo

The Windows tool for Modbus commissioning and fault finding: find every device on the line, test each point without
risk, and hand the client a report of what you proved.

**Product page, pricing and Pro licences:** https://coilo.kalkansoftware.com/ · **45-second tour:** https://youtu.be/aP_Ued_rUqw

This repository publishes Coilo's releases (downloads and release notes). The source code is not public. Coilo was
called ModbusTool up to version 2.2; profiles, point lists and licence keys from ModbusTool keep working in Coilo.

## Download

Get the latest files from [Releases](https://github.com/sabahattink/coilo-releases/releases/latest) or from the
[product page](https://coilo.kalkansoftware.com/):

- `Coilo-win-Setup.exe`: the installer, recommended; no admin rights needed.
- `Coilo-<version>-win-x64.zip`: portable; unzip and run.
- `ModbusSimulator.exe`: three Modbus TCP devices on your computer, to try Coilo without hardware.

Windows 10 or 11, 64-bit; no .NET to install. The files are not code-signed yet, so your browser may warn about the
download and Windows SmartScreen may stop the first start (More info → Run anyway). Check each file against
`SHA256SUMS.txt` in the release first:

```powershell
Get-FileHash .\Coilo-win-Setup.exe -Algorithm SHA256
```

## Free and Pro

| | Free | Pro |
|---|:---:|:---:|
| Modbus TCP, RTU over RS-485/RS-232, and RTU over TCP | ✓ | ✓ |
| Function codes 01–06, 15 and 16; eight data types, four byte orders | ✓ | ✓ |
| Writes locked until you unlock them, read back and checked, one-click undo | ✓ | ✓ |
| Slave ID scan with baud rate and parity detection, FC43 device identity | ✓ | ✓ |
| Polling from 100 ms to 60 s, trend, bit grid, labels, profiles, CSV export | ✓ | ✓ |
| Success rate, timeouts, exceptions and p95 latency per slave; raw frames | ✓ | ✓ |
| Commercial use, no time limit | ✓ | ✓ |
| Register map discovery | | ✓ |
| Point list: type, byte order, scale and unit per point; CSV in and out | | ✓ |
| Long-term recording to CSV | | ✓ |
| RS-485 bus monitor that listens without transmitting | | ✓ |
| Slave mode over Modbus TCP or RTU | | ✓ |
| Commissioning report (HTML, prints to PDF) | | ✓ |

Pro is 49 USD per seat, paid once (plus tax where it applies), with 12 months of updates; every version released in
that time keeps working without time limit. The key is checked on your computer: no account, no internet, no
activation server. 14-day refund, no questions asked. Paddle.com is the Merchant of Record for all orders.

Twelve languages, dark and light theme, works offline. No telemetry: besides your devices, Coilo contacts only GitHub,
to check for updates, and that can be turned off in About (F1).

## Safety

Coilo is a commissioning and diagnostic tool, not a control system. Writing is locked by default and is unlocked on
purpose; every write is yours to check on site.

Do not use Coilo to write to life-safety systems such as fire detection, fire suppression, voice evacuation, smoke
extraction or emergency lighting.

## Licence and support

Coilo is proprietary software, © 2026 Sabahattin Kalkan. Use is governed by the
[end user licence agreement](https://coilo.kalkansoftware.com/eula/).

Questions and bug reports: hello@kalkansoftware.com

Modbus® is a registered trademark of Schneider Electric USA, Inc. Coilo is not affiliated with or endorsed by Schneider
Electric or the Modbus Organization. Windows is a trademark of the Microsoft group of companies.
