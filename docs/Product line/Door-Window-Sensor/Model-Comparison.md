---
sidebar_position: 2
---

# Model Comparison

## Model Comparison

| Model | Protocol | Power | Battery Life | Features | Usage Suggestions |
|------|------|------|----------|------|----------|
| [HS1DS](../../无线协议/Zigbee/HS1DS-Door-Window-Sensor-Zigbee) | Zigbee / Z-Wave | CR1632 | 2-3 years | Standard, dual protocol optional | Open door turn on light, away arming, door/window illegal open push alert + siren linkage |
| [HS1DS-M](../../无线协议/Matter/HS1DS-M-Door-Window-Sensor-Matter-over-Thread) | Matter over Thread | CR1632 | 2-3 years | Matter version, cross-platform | Native Apple Home, away mode auto-check doors/windows then arm |

## Scenario Recommendations

| Scenario | Recommended Model | Automation Scheme |
|------|----------|----------|
| Arrival auto light | HS1DS | Door sensor detects open → turn on living room light → turn on AC → play welcome |
| Away arming | HS1DS | Door/window abnormal open detected → phone push + siren alarm linkage |
| Window rain protection linkage | HS1DS | Window open and rain sensor triggered → TTS broadcast remind close window |
| Apple Home users | HS1DS-M | Native Matter, HomeKit automation "last person leaving checks doors after closing" |
| Storage room/drawer monitoring | HS1DS | Compact size, detect cabinet/drawer illegal open, suitable for office/hotel |

## Selection Guide

- **Already have Zigbee gateway**: [HS1DS](../../无线协议/Zigbee/HS1DS-Door-Window-Sensor-Zigbee) (Zigbee version)
- **Need cross-platform compatibility**: [HS1DS-M](../../无线协议/Matter/HS1DS-M-Door-Window-Sensor-Matter-over-Thread) (Matter over Thread)
- **Z-Wave system**: [HS1DS](../../无线协议/Zigbee/HS1DS-Door-Window-Sensor-Zigbee) (Z-Wave version)
