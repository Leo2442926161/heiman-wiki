---
sidebar_position: 2
---

# Model Comparison

## Model Comparison

| Model | Protocol | Detection Gas | Certification | Power | Features | Usage Suggestions |
|------|------|----------|------|------|------|----------|
| JT-G1 | Standalone | Natural gas/LPG | GB 15322 | Mains | Independent audible/visual alarm | No gateway needed, built-in buzzer, basic gas leak alarm |
| [JT-HS1CG](../../无线协议/Zigbee/HS1CG-Gas-Detector-Zigbee) | Zigbee | Natural gas/LPG | GB 15322 | Mains | Zigbee networked | Leak detected → Zigbee notifies phone →linkage solenoid valve auto shutoff |
| [JT-HS3CG](../../无线协议/Zigbee/HS3CG-Gas-Detector-Zigbee) | Zigbee | Natural gas/LPG | GB 15322 | Mains | Enhanced | Higher sensitivity, supports remote valve shutoff + audible/visual alarm |
| JT-HS8CG | Zigbee / Wi-Fi | Natural gas/LPG | GB 15322 | Mains | Dual network | WiFi direct or Zigbee gateway, dual communication redundancy |
| [JT Series](../../无线协议/Zigbee/JT-Series-Gas-Emergency-Shutoff-Valve-Zigbee) | Zigbee | Natural gas/LPG | GB 15322 | Mains | General series | Multiple models available, adapts to different scenarios |

## Scenario Recommendations

| Scenario | Recommended Model | Automation Scheme |
|------|----------|----------|
| Kitchen safety automation | HS1CG / HS3CG | Leak detected → auto close solenoid valve → turn on exhaust fan → push notification →linkage siren |
| Rental/apartment | JT-G1 | Standalone alarm no networking needed, low cost, meets fire inspection requirements |
| Remote monitoring needs | HS8CG | Dual communication + cloud platform remote status viewing |
| Commercial kitchen | HS3CG | High sensitivity +linkage exhaust system + property platform centralized management |

## Selection Guide

- **Standalone use**: JT-G1
- **Zigbee networked**: [HS1CG](../../无线协议/Zigbee/HS1CG-Gas-Detector-Zigbee) or [HS3CG](../../无线协议/Zigbee/HS3CG-Gas-Detector-Zigbee)
- **Dual communication**: JT-HS8CG
