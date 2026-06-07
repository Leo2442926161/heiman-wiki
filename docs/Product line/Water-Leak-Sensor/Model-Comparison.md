---
sidebar_position: 2
---

# Model Comparison

## Model Comparison

| Model | Protocol | Detection Method | Power | Features | Usage Suggestions |
|------|------|----------|------|------|----------|
| [HS1WL](../../无线协议/Zigbee/HS1WL-Water-Leak-Detector-Zigbee) | Zigbee | Probe | Battery | Basic model | Leak triggers alarm push, suitable under bathroom sink |
| [HS2WL](../../无线协议/Zigbee/HS2WL-Water-Leak-Detector-Zigbee) | Zigbee | Probe + cable | Battery | Dual channel | Probe for spot detection + cable for long area coverage, best near water heater/washing machine |
| [HS3WL](../../无线协议/Zigbee/HS3WL-Water-Leak-Detector-Zigbee) | Zigbee | Probe | Battery | Enhanced version | Higher sensitivity, louder buzzer |
| [L1-M](../../无线协议/Matter/L1-M-Water-Leak-Detector-Matter) | Matter over Thread | Probe | Battery | Matter version | WWHA certified, native Apple Home integration |

## Scenario Recommendations

| Scenario | Recommended Model | Automation Scheme |
|------|----------|----------|
| Whole-house leak monitoring | HS2WL + L1-M | Multi-point coverage + native HomeKit notification, leak detected → close main water valve → push notification |
| Washing machine-dedicated | HS2WL | Cable probe laid under washing machine, immediate alarm on leak + cut washing machine power |
| Water heater/floor heating | HS3WL | Enhanced high sensitivity, detects floor heating pipe leaks early |
| Matter users | L1-M | No dedicated gateway needed, Thread low-latency alarm linkage Apple Home automation |

## Selection Guide

- **Spot detection**: [HS1WL](../../无线协议/Zigbee/HS1WL-Water-Leak-Detector-Zigbee) or [L1-M](../../无线协议/Matter/L1-M-Water-Leak-Detector-Matter)
- **Large area coverage**: [HS2WL](../../无线协议/Zigbee/HS2WL-Water-Leak-Detector-Zigbee) (probe + cable)
- **Matter needs**: [L1-M](../../无线协议/Matter/L1-M-Water-Leak-Detector-Matter)
