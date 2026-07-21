---
sidebar_position: 3
---







# Home Assistant Integration

The HS1SA-E and HS1SA-E Plus smoke alarms can be integrated locally into Home Assistant using either ZHA (Zigbee Home Automation) or Zigbee2MQTT (Z2M).

A compatible Zigbee coordinator is required. The available entities and controls may vary depending on the product model, firmware version, Home Assistant version, and the Zigbee integration being used.



## Supported Integrations

The following integrations are supported:

- ZHA (Zigbee Home Automation)
- Zigbee2MQTT
- Home Assistant automations
- Node-RED automations through Home Assistant or MQTT

All smoke detection and audible alarm functions continue to operate locally on the device. Smart home integration provides additional status reporting, remote controls, notifications, and automation capabilities.

------

# HS1SA-E

The HS1SA-E provides the essential smoke alarm information required for monitoring and automation.

## Available Functions

### Smoke Alarm Status

Indicates whether smoke has been detected.

When smoke is detected, the smoke alarm activates its local audible alarm and reports the alarm state to the connected Zigbee system.

This status can be used to trigger Home Assistant automations, including:

- Sending mobile notifications
- Turning on emergency lighting
- Activating additional sirens
- Unlocking evacuation routes
- Recording camera snapshots
- Shutting down ventilation systems

### Battery Level

Displays the estimated remaining battery capacity as a percentage.

The reported battery value can be used to create a maintenance reminder before the battery becomes critically low.

### Low-Battery Warning

Indicates that the battery is approaching the end of its usable capacity.

Replace the battery as soon as possible after a low-battery warning is received.

### Test Status

Indicates whether the smoke alarm is currently performing a local test.

The test status is normally activated when the physical test button on the smoke alarm is pressed.

## HS1SA-E Function Summary

| Function                     | ZHA           | Zigbee2MQTT   |
| ---------------------------- | ------------- | ------------- |
| Smoke detected status        | Supported     | Supported     |
| Battery percentage           | Supported     | Supported     |
| Low-battery warning          | Supported     | Supported     |
| Physical test status         | Supported     | Supported     |
| Home Assistant automations   | Supported     | Supported     |
| Remote self-test             | Not available | Not available |
| Remote mute                  | Not available | Not available |
| Temperature reporting        | Not available | Not available |
| Smoke level reporting        | Not available | Not available |
| Heartbeat indicator control  | Not available | Not available |
| Chamber contamination status | Not available | Not available |
| Remote siren control         | Not available | Not available |

------

# HS1SA-E Plus

The HS1SA-E Plus provides extended monitoring, control, interconnection, and diagnostic functions for advanced smart home applications.

Depending on the firmware version, the Zigbee model identifier may be displayed as `HS1SA-EF-3.0` or `HS1SA-E-PLUS`.

## Alarm and Safety Functions

### Smoke Alarm Status

Indicates whether the smoke alarm has detected smoke.

This is the primary alarm entity and can be used as a trigger in Home Assistant or Node-RED automations.

### Low-Battery Warning

Indicates that the remaining battery capacity is low and that the battery should be replaced.

### Test Status

Indicates whether the device is currently performing a self-test or physical button test.

### Fault Status

Reports whether the smoke alarm is operating normally or whether an internal fault has been detected.

The displayed fault information may vary depending on the integration and firmware version.

### Muted Status

Indicates whether the audible alarm is currently muted.

This entity reports the current mute state and should not be confused with the remote mute control.

------

## Remote Controls

### Remote Self-Test

Allows the user to start a smoke alarm self-test from Home Assistant or Zigbee2MQTT.

During the test, the device checks its audible alarm and internal alarm functions. Depending on the configured automation, the remote test may also be used to verify interconnected alarms.

Regular manual testing with the physical test button is still recommended.

### Temporary Mute

Allows the audible alarm to be temporarily silenced after the user has confirmed that there is no real fire.

**Warning:** Never mute the alarm until the protected area has been checked and it has been confirmed that there is no smoke or fire hazard.

The mute duration is controlled by the smoke alarm firmware. The alarm may automatically reactivate if smoke remains present or rises above the permitted mute threshold.

### Heartbeat Indicator

Allows the periodic status LED to be enabled or disabled.

Disabling the heartbeat indicator can be useful when the smoke alarm is installed in a bedroom or another area where periodic LED flashes may cause disturbance.

Disabling the heartbeat indicator does not disable smoke detection or the local audible alarm.

### Device Identification

Causes the device indicator to flash temporarily so that the selected smoke alarm can be physically identified.

This function is particularly useful when multiple smoke alarms are installed in the same Home Assistant system.

------

## Environmental Monitoring

### Temperature

Reports the ambient temperature measured near the smoke alarm.

Because the temperature sensor is located inside the product enclosure and close to the ceiling, the reported value may differ from the temperature measured by a room thermostat.

The temperature measurement is intended primarily for environmental monitoring and automation. It must not be used as a certified heat alarm.

### Temperature Offset

Allows a calibration offset to be applied to the reported temperature.

The supported adjustment range is from −15 °C to +15 °C in Zigbee2MQTT.

Use this setting only after comparing the smoke alarm temperature with a reliable reference thermometer under stable environmental conditions.

------

## Smoke Chamber Monitoring

### Smoke Level

Reports the current smoke concentration level measured by the optical smoke chamber.

This value can be used to create early-warning or pre-alarm automations before the main smoke alarm threshold is reached.

The smoke level must not be used to replace the certified smoke alarm state. The main smoke alarm entity remains the authoritative indication of a fire alarm condition.

### Smoke Unit

Zigbee2MQTT may expose the smoke concentration unit separately.

Possible units include:

- dB/m
- %/ft obscuration

The displayed unit depends on the device firmware and integration implementation.

### Chamber Contamination

Reports the estimated contamination condition of the optical smoke chamber.

Possible states include:

- Normal
- Light contamination
- Medium contamination
- Critical contamination

A contaminated chamber may affect long-term smoke detection performance. Clean the product according to the maintenance instructions. Replace the smoke alarm if a critical contamination condition remains after cleaning.

------

## Interconnection and Siren Functions

### Interconnectable Status

Indicates whether the smoke alarm supports use in an interconnection automation.

This status can be used by Home Assistant or Node-RED to identify devices that are suitable for coordinated alarm triggering.

### Link or Alarm Source Status

Reports the type of alarm involved in an interconnection event.

Depending on the platform, the available states may include:

- Inactive
- Smoke alarm active
- Carbon monoxide alarm active
- Heat alarm active

This information can help identify which alarm type initiated a whole-home warning.

### Siren Control

The HS1SA-E Plus can be activated as part of a Home Assistant automation.

Supported siren commands may include:

- Stop siren
- Smoke alarm sound
- Carbon monoxide alarm sound

This function allows multiple compatible alarms to sound together when smoke or carbon monoxide is detected elsewhere in the home.

Siren controls are intended for safety-related automations and system testing. They should not be used as general-purpose notification sounds.

The exact siren controls displayed in ZHA may differ from those displayed in Zigbee2MQTT.

------

## Diagnostic Information

The HS1SA-E Plus provides additional diagnostic information for monitoring Zigbee network stability and device operation.

### Reported Packages

Displays the number of Zigbee reports transmitted by the device during the reporting period.

An unusually high number may indicate frequent state changes, repeated reporting, or an automation configuration that requires investigation.

### Rejoin Count

Displays how many times the device has rejoined the Zigbee network.

A continuously increasing rejoin count may indicate:

- Weak Zigbee signal
- Insufficient Zigbee router coverage
- Coordinator instability
- Radio interference
- Zigbee network changes

### Reboot Count

Displays how many times the smoke alarm has restarted.

An unexpected increase may indicate battery contact problems, firmware restarts, or another device stability issue.

Some diagnostic entities may be disabled by default in ZHA. They can be enabled from the device entity settings when troubleshooting is required.

------

## HS1SA-E Plus Function Summary

| Function                          | ZHA                                  | Zigbee2MQTT                          |
| --------------------------------- | ------------------------------------ | ------------------------------------ |
| Smoke detected status             | Supported                            | Supported                            |
| Battery percentage                | Supported                            | Supported                            |
| Low-battery warning               | Supported                            | Supported                            |
| Test status                       | Supported                            | Supported                            |
| Fault status                      | Supported                            | Supported                            |
| Muted status                      | Supported                            | Supported                            |
| Remote self-test                  | Supported                            | Supported                            |
| Temporary remote mute             | Supported                            | Supported                            |
| Heartbeat indicator control       | Supported                            | Supported                            |
| Temperature reporting             | Supported                            | Supported                            |
| Smoke level reporting             | Supported                            | Supported                            |
| Chamber contamination status      | Supported                            | Supported                            |
| Interconnection capability status | Supported                            | Supported                            |
| Siren control for automations     | Supported                            | Supported                            |
| Smoke/CO alarm source information | Integration dependent                | Supported                            |
| Temperature offset                | Integration dependent                | Supported                            |
| Reported Zigbee packages          | Supported                            | Supported                            |
| Zigbee rejoin count               | Supported                            | Supported                            |
| Device reboot count               | Supported                            | Supported                            |
| Device identification             | Integration dependent                | Supported                            |
| OTA firmware updates              | Supported when firmware is available | Supported when firmware is available |

------

# Important Safety Information

Home Assistant, ZHA, Zigbee2MQTT, MQTT, mobile notifications, network connections, and automations are supplementary functions only.

The local smoke detection circuit, built-in audible alarm, physical test button, battery warning, installation requirements, and regular maintenance procedures remain the primary safety functions of the product.

Do not rely exclusively on:

- Mobile notifications
- Home Assistant automations
- Internet connectivity
- Zigbee connectivity
- Remote sirens
- Remote mute controls

Always install, test, clean, maintain, and replace the smoke alarm in accordance with the product safety manual and applicable local regulations.

Feature names and available controls may change after updates to Home Assistant, ZHA, Zigbee2MQTT, the device handler, or the smoke alarm firmware.



