---
layout: documentation
title: Ecolink PIR v2.5 - ZWave
---

{% include base.html %}

# Ecolink PIR v2.5 Z-Wave PIR Motion Sensor v2.5
This describes the Z-Wave device *Ecolink PIR v2.5*, manufactured by *Ecolink* with the thing type UID of ```eco_ecolinkpirv25_00_000```.

# Overview

**Overview:**

This is a hardware revision update to EcoLink's prior PIR sensor. It provides the same general capabilities as the prior detector--motion detection, battery state messages, and "burgler" alarm for the case being opened. On motion detection a green LED will flash and the notification will be sent to Group 1.

**Association Groups:**

The device has two association groups of up to 5 nodes each.

**Configuration Parameters:**

The device has two configuration parameters. Parameter 1 configures the sensor to send or not send Basic Set commands of 0x00 to nodes in Association group 2 turning the devices off when the sensor is in a restored state (i.e. motion not detected). By default the sensor does NOT send Basic Set commands of 0x00. Paremter 2 configures the sensor to either send or not to send Sensor Binary Report commands to Association Group 1 when the sensor is faulted and restored. If the controller is fully compatible with the Notification Command Class thereby making the Sensor Binary Reports redundant, the controller can disable the Sensor Binary Report Commands completely.

## Inclusion Information

Initial device inclusion is started by removing the pull tab from the back of the unit. This connects the battery and the device will immediately be eligible for inclusion. Place your controller in inclusion mode prior to pulling the tab from the back.

The manual indicates network-wide inclusion is supported, but also indicates that the device should be within 15 feet of the controller during the inclusion process.

## Channels

The following table summarises the channels available for the Ecolink PIR v2.5

| Channel | Channel Id | Category | Item Type |
|---------|------------|----------|-----------|
| Binary Sensor | sensor_binary | Door | Switch | 
| Alarm (power) | alarm_power | Door | Switch | 
| Alarm (burglar) | alarm_burglar | Door | Switch | 

### Binary Sensor

The ```sensor_binary``` channel supports the ```Switch``` item and is in the ```Door``` category. This is a read only channel so will only be updated following state changes from the device.

The following state translation is provided for this channel to the ```Switch``` item type -:

| Value | Label     |
|-------|-----------|
| ON | Triggered |
| OFF | Untriggered |

### Alarm (power)

The ```alarm_power``` channel supports the ```Switch``` item and is in the ```Door``` category. This is a read only channel so will only be updated following state changes from the device.

The following state translation is provided for this channel to the ```Switch``` item type -:

| Value | Label     |
|-------|-----------|
| OFF | Ok |
| ON | Alarm |

### Alarm (burglar)

The ```alarm_burglar``` channel supports the ```Switch``` item and is in the ```Door``` category. This is a read only channel so will only be updated following state changes from the device.

The following state translation is provided for this channel to the ```Switch``` item type -:

| Value | Label     |
|-------|-----------|
| OFF | Ok |
| ON | Alarm |



## Device Configuration

The following table provides a summary of the 2 configuration parameters available in the Ecolink PIR v2.5.
Detailed information on each parameter can be found in the sections below.

| Param | Name  | Description |
|-------|-------|-------------|
| 1 | Send Basic Sets | Send or do not send Basic Set commands to AG2 |
| 2 | Send Binary Reports | Send Sensor Binary Reports for backward compatibility |

### Parameter 1: Send Basic Sets

Send or do not send Basic Set commands to AG2
Parameter 1 configures the sensor to send or not send Basic Set commands of 0x00 to nodes in Association group 2 turning the devices off when the sensor is in a restored state (i.e. motion not detected). By default the sensor does NOT send Basic Set commands of 0x00.

Configuration Value: 0x00:

(Default) Sensor does NOT send Basic Sets to Node IDs in Association Group 2 when the sensor is restored (i.e. Motion Not Detected)

Configuration Value: 0xFF:

Sensor sends Basic Sets of 0x00 to nodes in Association Group2 when sensor is restored
The following option values may be configured -:

| Value  | Description |
|--------|-------------|
| 0 | Do not send |
| 255 | Send Basic Sets |

The manufacturer defined default value is 0 (Do not send).

This parameter has the configuration ID ```config_1_1``` and is of type ```INTEGER```.


### Parameter 2: Send Binary Reports

Send Sensor Binary Reports for backward compatibility
Paremter 2 configures the sensor to either send or not to send Sensor Binary Report commands to Association Group 1 when the sensor is faulted and restored. If the controller is fully compatible with the Notification Command Class thereby making the Sensor Binary Reports redundant, the controller can disable the Sensor Binary Report Commands completely.

Configuration Value: 0x00:

(Default) Sensor sends Sensor Binary Reports when sensor is faulted and restored for backwards compatibility in addition to Notification Reports.

Configuration Value: 0xFF:

Sensor will send only Notification Reports and NOT Sensor Binary Reports when the sensor is faulted and restored.
The following option values may be configured -:

| Value  | Description |
|--------|-------------|
| 0 | Send Sensor Binary Reports |
| 255 | Send only Notification Reports |

The manufacturer defined default value is 0 (Send Sensor Binary Reports).

This parameter has the configuration ID ```config_2_1``` and is of type ```INTEGER```.


## Association Groups

Association groups allow the device to send unsolicited reports to the controller, or other devices in the network. Using association groups can allow you to eliminate polling, providing instant feedback of a device state change without unnecessary network traffic.

The Ecolink PIR v2.5 supports 2 association groups.

### Group 1: Group 1


This group supports 5 nodes.

### Group 2: Group 2


This group supports 5 nodes.

## Technical Information

### Endpoints

#### Endpoint 0

| Command Class | Comment |
|---------------|---------|
| COMMAND_CLASS_NO_OPERATION_V1| |
| COMMAND_CLASS_BASIC_V1| |
| COMMAND_CLASS_SENSOR_BINARY_V2| |
| COMMAND_CLASS_ASSOCIATION_GRP_INFO_V1| |
| COMMAND_CLASS_DEVICE_RESET_LOCALLY_V0| |
| COMMAND_CLASS_ZWAVEPLUS_INFO_V1| |
| COMMAND_CLASS_CONFIGURATION_V1| |
| COMMAND_CLASS_ALARM_V5| |
| COMMAND_CLASS_MANUFACTURER_SPECIFIC_V1| |
| COMMAND_CLASS_POWERLEVEL_V1| |
| COMMAND_CLASS_BATTERY_V1| |
| COMMAND_CLASS_WAKE_UP_V2| |
| COMMAND_CLASS_ASSOCIATION_V2| |
| COMMAND_CLASS_VERSION_V2| |

---

Did you spot an error in the above definition or want to improve the content?
You can [edit the database here](http://www.cd-jackson.com/index.php/zwave/zwave-device-database/zwave-device-list/devicesummary/525).
