---
sidebar_position: 2
---

# Model Comparison

## Model Comparison

| Model | Protocol | Detection Angle | Mounting | Features | Usage Suggestions |
|------|------|----------|------|------|----------|
| [HS1MS](../../无线协议/Zigbee/HS1MS-PIR-Sensor-Zigbee) | Zigbee | 110° | Wall | Basic model, economical | Lights on/off with motion, security linkage motion detection push alert |
| [HS3MS](../../无线协议/Zigbee/HS3MS-PIR-Sensor-Zigbee) | Zigbee | 360° | Ceiling | Full coverage | Ceiling full coverage no blind spots, ideal for living rooms/lobby areas |
| [M1-Z](../../无线协议/Zigbee/M1-Z-PIR-Sensor-Zigbee) | Zigbee | 110° | Wall | Light level detection | PIR + light sensor: no light-off during daytime, auto on at night |
| [M1-M](../../无线协议/Matter/M1-M-PIR-Sensor-Matter) | Matter over Thread | 110° | Wall | Matter version | Native HA + Apple Home, light level linkage curtains auto adjust |
| [HS8MLS](../../无线协议/Zigbee/HS8MLS-Micro-Motion-Sensor-Zigbee) | Zigbee | 110° | Wall | Long range | Corridors/garages long straight areas, longer detection distance |
| [HS8MIS](../../无线协议/Zigbee/HS8MIS-Motion-Sensor-Zigbee) | Zigbee | 110° | Wall | Combined sensor | PIR + light level 2-in-1,linkage smart light brightness based on ambient light |

## Scenario Recommendations

| Scenario | Recommended Model | Automation Scheme |
|------|----------|----------|
| Motion-activated energy saving | M1-Z / HS8MIS | PIR detects person → turn on light + read illuminance for brightness → timeout off |
| Security arming linkage | HS1MS | Away mode detects motion → push alert + siren + camera recording |
| Ceiling full coverage | HS3MS | Center ceiling mount, 360° no blind spots, ideal for open spaces |
| Matter cross-ecosystem | M1-M | Apple Home automation + Google/Alexa voice, light linkage curtains |
| Long corridor/garage | HS8MLS | Long distance detection, auto lighting for vehicle/personnel entry/exit |

## Selection Guide

- **Corridor/room wall mount**: [HS1MS](../../无线协议/Zigbee/HS1MS-PIR-Sensor-Zigbee) or [HS8MLS](../../无线协议/Zigbee/HS8MLS-Micro-Motion-Sensor-Zigbee) (long range)
- **Ceiling full coverage**: [HS3MS](../../无线协议/Zigbee/HS3MS-PIR-Sensor-Zigbee) (360°)
- **Need light level**: [M1 Series](../../无线协议/Zigbee/M1-Z-PIR-Sensor-Zigbee) or [HS8MIS](../../无线协议/Zigbee/HS8MIS-Motion-Sensor-Zigbee)
- **Matter platform**: [M1-M](../../无线协议/Matter/M1-M-PIR-Sensor-Matter)
