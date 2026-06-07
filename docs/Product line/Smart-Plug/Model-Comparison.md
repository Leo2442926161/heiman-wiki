---
sidebar_position: 2
---

# Model Comparison

## Model Comparison

| Model | Protocol | Rated Power | Metering Accuracy | Features | Usage Suggestions |
|------|------|----------|----------|------|----------|
| [HS2SK](../../无线协议/Zigbee/HS2SK-Smart-Plug-Zigbee) | Zigbee | 16A / 3680W | ±2% | Metering type | Real-time power monitoring + remote on/off,linkage away mode one-click power-off, track AC/water heater energy usage |
| [HS2SK-WiFi](../../无线协议/Wifi/HS2SK-WiFi-Smart-Metering-Plug-WiFi) | WiFi | 16A / 3680W | ±2% | Direct connect no gateway needed | No extra gateway, Smart Life App direct control, ideal for users who don't want to buy a gateway |

## Scenario Recommendations

| Scenario | Recommended Model | Automation Scheme |
|------|----------|----------|
| Energy monitoring | HS2SK | Zigbee connect to HA,linkage InfluxDB + Grafana display daily/monthly energy usage, identify high-consumption appliances |
| Away power-off | HS2SK | Away mode one-click turn off TV/AC/aquarium light, safe and energy-saving |
| Timer control | HS2SK / HS2SK-WiFi | Timer on/off water heater/humidifier/charger, optimize with peak/off-peak electricity pricing |
| No gateway users | HS2SK-WiFi | Direct connect to router, Smart Life App control, zero learning curve |

## Selection Guide

- **Already have Zigbee gateway**: [HS2SK](../../无线协议/Zigbee/HS2SK-Smart-Plug-Zigbee)
- **Don't want to buy gateway**: [HS2SK-WiFi](../../无线协议/Wifi/HS2SK-WiFi-Smart-Metering-Plug-WiFi)
