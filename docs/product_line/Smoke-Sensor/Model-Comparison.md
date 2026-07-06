---
sidebar_position: 2
---

# Model Comparison

## Model Comparison

| Model | Protocol | Certification | Power | Market | Usage Suggestions |
|------|------|------|------|------|----------|
| [HS1SA-E](../../protocol/Zigbee/HS1SA-E-Zigbee-Smoke-Alarm/) | Zigbee | EN 14604 | CR123A | EU | Integrate with Zigbee2MQTT/ZHA, Home Assistant automation — auto-turn on lights + push notification when smoke detected |
| HS1SA-Z | Z-Wave | EN 14604 | CR123A | EU | Connect to SmartThings/Hubitat, arm with Z-Wave door sensor, smoke alarm auto-notify when away |
| [HS1SA-M](../../protocol/Matter/HS1SA-M-Smoke-Alarm-Matter/) | Matter over Thread | EN 14604 | CR123A | Global | Native Apple Home/Google Home integration, no dedicated gateway needed, low-latency Thread local alarm linkage |
| HS3SA | Zigbee | EN 14604 | CR123A | EU | Use with Heiman HS6GW gateway, multi-device scene linkage, ideal for Heiman ecosystem users |
| HS8SA | Zigbee / Wi-Fi | UL 217 | Battery/Mains | US | US market-dedicated, UL certified, meets local fire codes, supports WiFi direct or Zigbee gateway |
| S1 Series | Sub-1G | EN 14604 | Battery | Universal | Standalone-interconnected, no gateway or internet needed, Sub-1G wireless interconnection between units, ideal for simple rentals |

## Scenario Recommendations

| Scenario | Recommended Model | Automation Scheme |
|------|----------|----------|
| Deep smart home integration | HS1SA-E / HS1SA-M | HA automation: smoke alarm → turn on all lights → unlock door → close gas valve → push notification |
| Apple HomeKit users | HS1SA-M | Native Matter integration, HomePod as Thread border router, automatic scene triggers |
| EU/US standard requirements | HS1SA-E (CE) / HS8SA (UL) | Meets local fire certifications, insurance compliance |
| No gateway / low cost | S1 Series | Buy and use, Sub-1G interconnection between units, mutual triggering on alarm |
| Existing Z-Wave system | HS1SA-Z | Use with existing Z-Wave gateway like Hubitat/SmartThings |

## Selection Guide

- **EU market**: [HS1SA-E](../../protocol/Zigbee/HS1SA-E-Zigbee-Smoke-Alarm/) (Zigbee) or HS3SA (Zigbee), choose HS1SA-Z for Z-Wave
- **US market**: HS8SA (UL 217 certified)
- **Cross-platform Matter**: [HS1SA-M](../../protocol/Matter/HS1SA-M-Smoke-Alarm-Matter/) (Matter over Thread)
- **Standalone scenario**: S1 Series (no gateway needed)
