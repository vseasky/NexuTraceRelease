# NexuTrace

**NexuTrace** 是一款专业的多协议通信调试与数据可视化工具，面向嵌入式开发、物联网及工业应用场景。本仓库**单次发版交付两个产品**：

- **NexuTrace** —— 全功能版本，覆盖所有连接方式与协议。
- **VCAN-Views** —— USB-CAN 专用免费版本。保留全部数据分析视图，仅去掉非 USB-CAN 通道、在线升级器与订阅系统。

两个产品**统一发版**，每次提供 **Windows x64 + x86 (32 位) 两种架构**，共 4 个 zip 安装包。

## 连接方式

| 类型 | NexuTrace | VCAN-Views | 说明 |
|---|:---:|:---:|---|
| Serial | ✓ | — | COM 串口通信 |
| USB CDC | ✓ | — | 虚拟串口 (CDC ACM) |
| USB HID | ✓ | — | HID 设备通信 |
| USB WinUSB | ✓ | — | WinUSB 设备通信 |
| TCP Server | ✓ | — | TCP 服务端，支持多客户端 |
| TCP Client | ✓ | — | TCP 客户端连接 |
| UDP | ✓ | — | UDP 数据报通信 |
| **USB-CAN (VCAN)** | ✓ | ✓ | VCAN 协议，单/双通道 |
| **USB-CAN (Candle)** | ✓ | ✓ | Candle / gs_usb，双通道 + CAN-FD |

## 协议支持

| 协议 | 说明 |
|---|---|
| NexuFrame | 原生二进制协议，帧结构 + CRC 校验（USB-CAN 默认） |
| JustFloat | VOFA+ 兼容，小端浮点字节流 |
| FireWater | VOFA+ 兼容，CSV 文本解析 |

## 功能视图（双产品都支持）

### 发送视图
- 单条发送，支持 HEX / 文本模式
- 多条发送表格，每行独立配置通道、使能、周期、次数
- 周期发送，可配置发送间隔
- 自增计数前缀
- 换行类型选择 (NULL / LF / CR / CRLF)

### 接收视图
- 实时文本显示，高性能大文本渲染
- 行级选中与 Ctrl+C 复制
- 时间戳显示
- 自动滚动与暂停

### 接收表格视图
- 结构化数据包显示：TimeDelta、Time、ID、Direction、Type、Length、Data
- 行选中与滚动
- 冻结表头行

### HEX 分析器
- 十六进制 / ASCII 双面板显示
- 数据检查器 (uint8/16/32/64, int8/16/32/64, float, double, color)
- GoTo 导航 (偏移 / 行)

### 数据管理面板
- 数据记录表格，支持删除/发送按钮
- 表头列宽自适应

### 波形视图
- 多通道实时波形渲染
- Y 轴范围与显隐可配

### 仪表控件集（11 个）
- 电池、温度、音量、标尺、仪表盘、LED 灯、开关、数字显示、数值输入、标签图、波形
- 拖拽布局、主题适配、重启状态恢复

### 3D 视图
- 基于 Assimp 的 3D 模型渲染
- 场景配置走 JSON 文件

## 编码

统一的 VekEncoding 模块 — 支持 26 种文本编码。发送与接收视图按配置自动转码。

## 运行平台

| 操作系统 | 架构 |
|---|---|
| Windows 10 / 11 | x64 + x86 (32 位, Win32) |

## 源码

<https://github.com/vseasky/NexuTrace>

## 发版镜像（国内）

<https://gitee.com/vseasky/NexuTraceRelease>
