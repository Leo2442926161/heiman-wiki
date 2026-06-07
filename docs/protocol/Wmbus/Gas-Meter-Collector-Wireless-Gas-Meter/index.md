---
sidebar_position: 4
---

# Gas Collector - Wireless Gas Meter Data Collector

## Overview

The gas collector is a wM-Bus wireless data collection device launched by Heiman for the smart gas sector. It operates in the 868 MHz band (EN 13757 standard) and is used for remotely reading gas meter metering data and uploading it to a centralized meter reading system. Powered by an industrial-grade lithium battery with a battery life of 6~10 years, it is suitable for centralized meter reading scenarios in apartments, residential communities, commercial buildings, etc.

## Technical Specifications

| Parameter | Value |
|-----------|-------|
| Communication Protocol | wM-Bus (EN 13757) |
| Operating Frequency | 868 MHz (European SRD band) |
| Transmission Rate | 4.8 kbps / 16.384 kbps / 100 kbps (T/S/R modes) |
| Communication Range | Indoor approx. 100~300 m, open area approx. 500~1000 m |
| Power Supply | Industrial lithium battery (ER18505 / ER26500) |
| Battery Life | 6~10 years (typical reporting 1 time/day) |
| Operating Temperature | -20°C ~ +60°C |
| Operating Humidity | ≤ 95% RH |
| Protection Rating | IP65 ~ IP68 (depending on installation environment) |
| Data Encryption | AES-128 (optional) |

## Features

- Supports wM-Bus S/T/R three operating modes
- Automatically collects gas meter usage data and reports periodically
- Low power deep sleep, extended battery life
- AES-128 data encryption, ensuring communication security
- Supports remote firmware upgrade
- Reconnection and data retransmission mechanism
- Supports EN 13757-3 application layer protocol
- Can work with HS1-CM collector / HS1-GW gateway for centralized upload

## Certification Standards

- EN 13757-4 (Wireless M-Bus Physical Layer)
- EN 13757-3 (M-Bus Application Layer)
- CE / RED

## Related Documents

- See [wM-Bus Technical Parameters](../Technical-Specifications.md)
