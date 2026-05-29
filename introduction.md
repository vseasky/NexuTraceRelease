# NexuTrace

**NexuTrace** is a professional multi-protocol communication debugging and data visualization tool for embedded development, IoT, and industrial applications. The full distribution ships two products from one source tree:

- **NexuTrace** — full feature set, supports every connection type and protocol.
- **VCAN-Views** — USB-CAN dedicated free variant. All data analysis views are preserved; only the non-USB-CAN transports, online updater and subscription system are removed.

Both products are released **per version, in x64 + x86 (32-bit) Windows builds**, four zip files per release.

## Connectivity

| Type | NexuTrace | VCAN-Views | Description |
|---|:---:|:---:|---|
| Serial | ✓ | — | COM port communication |
| USB CDC | ✓ | — | Virtual serial port (CDC ACM) |
| USB HID | ✓ | — | HID device communication |
| USB WinUSB | ✓ | — | WinUSB device communication |
| TCP Server | ✓ | — | TCP server, multi-client support |
| TCP Client | ✓ | — | TCP client connection |
| UDP | ✓ | — | UDP datagram |
| **USB-CAN (VCAN)** | ✓ | ✓ | VCAN protocol, single/dual channel |
| **USB-CAN (Candle)** | ✓ | ✓ | Candle / gs_usb, dual channel + CAN-FD |

## Protocol Support

| Protocol | Description |
|---|---|
| NexuFrame | Native binary protocol with framing and CRC (default for USB-CAN) |
| JustFloat | VOFA+ compatible, little-endian float stream |
| FireWater | VOFA+ compatible, CSV text parsing |

## Views (available on both products)

### Transmit View
- Single send with HEX / text mode
- Multi-line send table with per-row channel, enable, period, count
- Periodic send with configurable interval
- Auto-increment prefix
- Newline style selection (NULL / LF / CR / CRLF)

### Receive View
- Real-time text display, optimized for large-volume rendering
- Per-line selection + Ctrl+C copy
- Timestamps
- Auto-scroll with pause

### Receive Table View
- Structured frames: TimeDelta / Time / ID / Direction / Type / Length / Data
- Row selection + scroll
- Frozen header row

### HEX Analyzer
- Hex / ASCII dual panel
- Data inspector (uint8/16/32/64, int8/16/32/64, float, double, color)
- Goto navigation (offset / row)

### Data Panel
- Editable data record table with delete / send buttons
- Auto-fit column widths

### Plot View
- Real-time waveform across multiple channels
- Configurable Y axis hint and visibility

### Widget Cluster (11 widgets)
- Battery, Temperature, Volume, Ruler, Gauge, LedBulb, ToggleSwitch, DigitDisplay, ValueInput, LabelImage, Plot
- Drag-resize layout, theming, persistence across restarts

### 3D View
- 3D model preview powered by Assimp
- Scene configurable via JSON

## Encoding

Unified VekEncoding module — 26 text encodings supported. Transmit and Receive views auto-encode per setting.

## Platform

| OS | Arch |
|---|---|
| Windows 10 / 11 | x64 + x86 (32-bit, Win32) |

## Source

<https://github.com/vseasky/NexuTrace>

## Release Mirror (China)

<https://gitee.com/vseasky/NexuTraceRelease>
