---
sidebar_position: 2
---

# Model Comparison

## Model Comparison

| Model | Protocol | Accuracy | Power | Features | Usage Suggestions |
|------|------|------|------|------|----------|
| [H1-M](../../无线协议/Matter/H1-M-Temp-Humidity-Sensor-Matter) | Matter over Thread | ±0.3°C / ±3% RH | CR2 | Matter version, cross-platform | Native Apple Home,linkage AC/floor heating to auto-adjust room temperature, auto-turn on exhaust fan when humidity high |
| H1-Z | Zigbee | ±0.3°C / ±3% RH | CR2 | Zigbee version | Connect to HA/Z2M, temperature anomaly alarm (notify if elderly home too cold/hot) |

## Scenario Recommendations

| Scenario | Recommended Model | Automation Scheme |
|------|----------|----------|
| Apple Home ecosystem | H1-M | Native Matter integration, HomeKit automation: temp > 28°C turn on AC, humidity > 70% turn on exhaust |
| HA power users | H1-Z or H1-M | HA automation: temp/humidity linkage floor heating/humidifier/dehumidifier, historical data InfluxDB + Grafana |
| Wine cellar/cigar cabinet | H1-Z | Temp/humidity out-of-range alarm + phone push, protect collectibles |
| Nursery monitoring | H1-M | Temp too high/low push notification,linkage AC to adjust to comfortable range |
| Plant greenhouse | H1-Z | Temp/humidity trigger auto-irrigation/ventilation/sunshade |

## Selection Guide

- **Matter cross-platform**: [H1-M](../../无线协议/Matter/H1-M-Temp-Humidity-Sensor-Matter)
- **Existing Zigbee system**: H1-Z
