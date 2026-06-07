---
sidebar_position: 11
---

# ZHA（Zigbee Home Automation）

ZHA is the built-in Zigbee integration for Home Assistant, allowing direct management of Zigbee devices without additional software.

## Compatibility

Heiman Zigbee sensors have excellent compatibility with ZHA, supporting:

- **Smoke/CO Alarm**: Alarm status, fault detection, battery level, silence
- **Door/Window Sensor**: Open/close, tamper
- **PIR Sensor**: Motion detection, illuminance
- **Temperature & Humidity**: Temperature, humidity
- **Water Leak**: Water leak alarm
- **Smart Plug**: On/off, power metering

## Hardware Requirements

- Zigbee Coordinator: HUSBZB-1, Conbee II, SkyConnect, SLZB-06, etc.
- Connected to Home Assistant via USB or network

## Configuration

ZHA configuration is simple — select the serial port and region, and it will automatically scan and discover devices. No manual configuration file editing required.

> **Reference**: [Home Assistant ZHA Documentation](https://www.home-assistant.io/integrations/zha/)
