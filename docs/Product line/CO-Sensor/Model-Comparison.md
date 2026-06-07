---
sidebar_position: 2
---

# Model Comparison

## Model Comparison

| Model | Protocol | Sensor | Certification | Power | Market | Usage Suggestions |
|------|------|--------|------|------|------|----------|
| [HS1CA-E](../../无线协议/Zigbee/HS1CA-E-CO-Alarm-Zigbee) | Zigbee | Electrochemical | EN 50291 | CR123A | EU | Integrate with Zigbee2MQTT, real-time CO monitoring, auto-shutoff gas boiler + open window exhaust + phone alert when threshold exceeded |
| [HS1CA-Z](../../无线协议/Zwave/HS1CA-Z-CO-Alarm-Z-Wave) | Z-Wave | Electrochemical | EN 50291 | CR123A | EU | Use with SmartThings/Hubitat, CO alarm triggers siren, ideal for experienced Z-Wave users |
| [HS1CA-M](../../无线协议/Matter/HS1CA-M-CO-Alarm-Matter) | Matter over Thread | Electrochemical | EN 50291 | CR123A | Global | World's first Matter CO alarm, Home Assistant official certified, no proprietary gateway needed |
| HS-720ES-M | Matter over Thread | Electrochemical | UL 2034 | CR123A | US | US market Matter CO alarm, UL 2034 certified, meets local fire codes |
| [C1 Series](../../无线协议/Zigbee/C1-Series-CO-Alarm-Zigbee) | Zigbee | Electrochemical | EN 50291 | CR123A | EU | Basic CO alarm, reliable functionality, best value |

## Scenario Recommendations

| Scenario | Recommended Model | Automation Scheme |
|------|----------|----------|
| Whole home smart safety | HS1CA-M | Matter over Thread native Apple Home + Google + Alexa, alarm → close gas → open windows |
| EU standard requirements | HS1CA-E | Connect to HA via Z2M/ZHA, auto-shutoff gas solenoid valve |
| US standard requirements | HS-720ES-M | UL 2034 certified, meets insurance requirements |
| Low-cost upgrade for older homes | C1 Series | Basic functions, use with gateway |

## Selection Guide

- **Matter cross-platform**: [HS1CA-M](../../无线协议/Matter/HS1CA-M-CO-Alarm-Matter) (global version, HA officially certified)
- **EU market**: [HS1CA-E](../../无线协议/Zigbee/HS1CA-E-CO-Alarm-Zigbee) (Zigbee)
- **US market**: HS-720ES-M (UL 2034)
- **Basic needs**: [C1 Series](../../无线协议/Zigbee/C1-Series-CO-Alarm-Zigbee) (Zigbee)
