---
sidebar_position: 1
---

# Home Assistant

In February 2026, Heiman Technology officially joined the **Works with Home Assistant** certification program, becoming one of the first Chinese partners in the program.

## Certified Devices

The following Heiman devices have been officially certified to ensure localized and stable compatibility with Home Assistant:

| Device | Region | Connection |
|------|------|----------|
| Smart Smoke Alarm | United States | Matter over Thread |
| Smart Smoke Alarm | EU / China | Matter over Thread |
| Smart Carbon Monoxide Alarm | United States | Matter over Thread |
| Smart Carbon Monoxide Alarm | EU / China | Matter over Thread |
| PIR Sensor M1 Series | Global | Matter / Zigbee |
| Water Leak Detector L1 Series | Global | Matter / Zigbee |
| Temperature & Humidity Sensor H1 Series | Global | Matter / Zigbee |

## Integration

### Via Matter

1. Ensure you have a Matter over Thread border router (e.g. Home Assistant Green + Connect ZBT-2, Apple HomePod, Google Nest Hub, etc.)
2. Configure the Matter integration in Home Assistant
3. Add the device and it will be automatically discovered

### Via Zigbee2MQTT / ZHA

Heiman Zigbee devices are natively supported by Zigbee2MQTT and ZHA, no additional configuration required.

## Local Control

All certified devices support **local control** with no dependency on cloud services. Even if the internet is down, sensor alarms and automation actions continue to function normally.

## Community Engagement

Heiman actively participates in discussions within the Home Assistant community and continuously improves product experience based on user feedback.

> **Reference**: [Home Assistant Official Announcement - Heiman joins Works with Home Assistant](https://www.home-assistant.io/blog/2026/02/24/heiman-joins-works-with-home-assistant/)
