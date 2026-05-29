# NexuTrace

> Multi-protocol communication debugging & data visualization toolkit for embedded development, IoT and industrial applications.

Two products share the same source tree and ship together:

| Product | Use case | Connections | License |
|---|---|---|---|
| **NexuTrace** | Full-stack debugging workbench | Serial / USB CDC / HID / WinUSB / TCP / UDP / **USB-CAN** | Subscription |
| **VCAN-Views** | USB-CAN dedicated toolkit | **USB-CAN only** (VCAN + Candle) | **Free** |

VCAN-Views keeps all data visualization capabilities (Hex / Plot / 11 widgets / DataPanel / 3D view); only the non-USB-CAN transports, online updater and subscription system are removed.

## Downloads

Every release ships **4 zip artifacts** (x64 + x86 for both products):

```
NexuTrace_x64_X_Y_Z_W.zip
NexuTrace_x86_X_Y_Z_W.zip
VCAN-Views_x64_X_Y_Z_W.zip
VCAN-Views_x86_X_Y_Z_W.zip
```

Grab the matching zip from the [Releases](https://github.com/vseasky/NexuTraceRelease/releases) page, extract and run the `.exe`.

## Documents

| File | Content |
|---|---|
| `introduction.md` | Feature overview, supported connections & protocols, view list |
| `release_history.md` | Per-version changelog (latest on top) |
| `zh/*` | Chinese versions of the above |

## Resources

- Source repository: <https://github.com/vseasky/NexuTrace>
- Release mirror (China): <https://gitee.com/vseasky/NexuTraceRelease>

## License

See [LICENSE](LICENSE).
