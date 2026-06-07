---
sidebar_position: 3
---

# Technical Parameters

The following are the general technical parameters of Heiman wireless M-Bus (wM-Bus) devices.

## Wireless Parameters

| Parameter | Value |
|-----------|-------|
| Protocol Standard | EN 13757-4 (Wireless M-Bus Physical Layer) |
| Operating Frequency | 868 MHz (European SRD band, 868.0~868.6 MHz) |
| Modulation | FSK |
| Transmission Rate | 4.8 kbps / 16.384 kbps / 100 kbps (T mode / S mode / R mode) |
| Network Topology | Star (Meter → Collector / Gateway) |
| Communication Range | Indoor approx. 100~300 m, open area approx. 500~1000 m |
| Transmit Power | ≤ 25 mW (+14 dBm) |

## Operating Modes

| Mode | Rate | Description |
|------|------|-------------|
| S mode | 16.384 kbps | Standard mode, low power, suitable for battery-powered meters |
| T mode | 100 kbps | High-speed mode, suitable for high data volume scenarios |
| R mode | 4.8 kbps | Narrowband mode, long-distance transmission |

## Electrical and Power Consumption

| Parameter | Value |
|-----------|-------|
| Power Supply | Lithium battery powered (ER18505 / ER26500 industrial lithium batteries) |
| Battery Life | 6~10 years (depending on reporting frequency, typical 1 time/day) |
| Standby Power Consumption | Microamp level, deep sleep |
| Receive Sensitivity | Approx. -105 dBm (S mode) |

## Environmental Parameters

| Parameter | Value |
|-----------|-------|
| Operating Temperature | -20°C ~ +60°C (industrial grade) |
| Operating Humidity | ≤ 95% RH (non-condensing) |
| IP Rating | IP65 ~ IP68 (depending on model, suitable for outdoor meters) |

## Data Protocol

| Layer | Standard |
|-------|----------|
| Physical Layer | EN 13757-4 |
| Data Link Layer | EN 13757-4 (Wireless M-Bus Frame Format) |
| Application Layer | EN 13757-3 (M-Bus Application Layer) |
| Encryption | AES-128 (optional encryption) |
