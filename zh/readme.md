# NexuTrace

> 面向嵌入式、物联网与工业场景的多协议通信调试与数据可视化工具。

同源同构，单次发版交付**两个产品**：

| 产品 | 定位 | 连接方式 | 授权 |
|---|---|---|---|
| **NexuTrace** | 全栈调试工作台 | Serial / USB CDC / HID / WinUSB / TCP / UDP / **USB-CAN** | 订阅制 |
| **VCAN-Views** | USB-CAN 专用工具 | **仅 USB-CAN**（VCAN + Candle） | **完全免费** |

VCAN-Views 保留全部数据可视化能力（Hex / Plot / 11 仪表控件 / 数据面板 / 3D 视图），仅去掉非 USB-CAN 通道、在线升级与订阅系统。

## 下载

每个版本提供 **4 个 zip 安装包**（双产品 × x64 + x86）：

```
NexuTrace_x64_X_Y_Z_W.zip
NexuTrace_x86_X_Y_Z_W.zip
VCAN-Views_x64_X_Y_Z_W.zip
VCAN-Views_x86_X_Y_Z_W.zip
```

到 [Releases](https://gitee.com/vseasky/NexuTraceRelease/releases) 页面下载对应 zip，解压后运行 `.exe` 即可。

## 文档

| 文件 | 内容 |
|---|---|
| `introduction.md` | 功能概览、支持的连接与协议、视图清单 |
| `release_history.md` | 历史发版日志（最新在顶部） |

英文版位于上一级目录。

## 资源

- 源码仓库：<https://github.com/vseasky/NexuTrace>
- 发版镜像（国内）：<https://gitee.com/vseasky/NexuTraceRelease>

## 许可

见 [LICENSE](../LICENSE)。
