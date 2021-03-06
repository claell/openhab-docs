---
layout: documentation
title: DMMZ1 - ZWave
---

{% include base.html %}

# DMMZ1 Dome Battery powered Z-Wave Plus enabled mousetrap
This describes the Z-Wave device *DMMZ1*, manufactured by *Elexa Consumer Products Inc.* with the thing type UID of ```elexa_dmmz1_00_000```.

# Overview


## Channels

The following table summarises the channels available for the DMMZ1

| Channel | Channel Id | Category | Item Type |
|---------|------------|----------|-----------|
| Binary Sensor | sensor_binary | Door | Switch | 
| Alarm | alarm_general | Door | Switch | 

### Binary Sensor

The ```sensor_binary``` channel supports the ```Switch``` item and is in the ```Door``` category. This is a read only channel so will only be updated following state changes from the device.

The following state translation is provided for this channel to the ```Switch``` item type -:

| Value | Label     |
|-------|-----------|
| ON | Triggered |
| OFF | Untriggered |

### Alarm

The ```alarm_general``` channel supports the ```Switch``` item and is in the ```Door``` category. This is a read only channel so will only be updated following state changes from the device.

The following state translation is provided for this channel to the ```Switch``` item type -:

| Value | Label     |
|-------|-----------|
| OFF | Ok |
| ON | Alarm |



## Device Configuration

The following table provides a summary of the 5 configuration parameters available in the DMMZ1.
Detailed information on each parameter can be found in the sections below.

| Param | Name  | Description |
|-------|-------|-------------|
| 1 | BASIC_SET Level | Sets the value sent by the BASIC\_SET command to Association Group 2 |
| 2 | Set Firing Mode | This parameter sets the “firing mode” of the Mouser. |
| 3 | High Voltage Duration Time  | How long the Mouser will fire continuously before it starts to burst-fire |
| 4 | Enable/Disable LED Alarm | Enables or disables the indicator LED alarm when the trap is tripped |
| 5 | LED Alarm Duration | Sets the amount of time the LED Indicator blinks after the trap is tripped |

### Parameter 1: BASIC_SET Level

Sets the value sent by the BASIC\_SET command to Association Group 2
This parameter sets the value sent by the BASIC\_SET command to Association Group 2 (for more information, see “Assocation Groups”.)

00 (0/Turn Off Device)

01 ~ 63 (0-99)

FF (255/Turn On Device)
Values in the range 0 to 255 may be set.

The manufacturer defined default value is 255.

This parameter has the configuration ID ```config_1_1``` and is of type ```INTEGER```.


### Parameter 2: Set Firing Mode

This parameter sets the “firing mode” of the Mouser.
This parameter sets “firing mode” of the Mouser. Two firing modes are available: in the first (Continuous Fire,) electricity is passed continuously for the entire duration, and in the second (Burst Fire,) electricity is passed continuously only for the first minute and it is pulsed at approximately 400 beats per minute for the remainder of the time.

01 (Continuous Fire)

02 (Burst Fire)
The following option values may be configured -:

| Value  | Description |
|--------|-------------|
| 1 | Continuous Fire |
| 2 | Burst Fire |

The manufacturer defined default value is 2 (Burst Fire).

This parameter has the configuration ID ```config_2_1``` and is of type ```INTEGER```.


### Parameter 3: High Voltage Duration Time 

How long the Mouser will fire continuously before it starts to burst-fire
This parameter defines how long the Mouser will fire continuously before it starts to burst-fire (see parameter 2.)

00 64 ~ 01 68 (100~360 in Seconds)
Values in the range 64 to 168 may be set.

The manufacturer defined default value is 64.

This parameter has the configuration ID ```config_3_2``` and is of type ```INTEGER```.


### Parameter 4: Enable/Disable LED Alarm

Enables or disables the indicator LED alarm when the trap is tripped
This parameter enables or disables the indicator LED alarm when the trap is tripped.

00 (LED Alarm Disabled)

01 (LED Alarm Enabled)
The following option values may be configured -:

| Value  | Description |
|--------|-------------|
| 0 | LED Alarm Disabled |
| 1 | LED Alarm Enabled |

The manufacturer defined default value is 1 (LED Alarm Enabled).

This parameter has the configuration ID ```config_4_1``` and is of type ```INTEGER```.


### Parameter 5: LED Alarm Duration

Sets the amount of time the LED Indicator blinks after the trap is tripped
This parameter sets the amount of time the LED Indicator blinks after the trap is tripped.

00 (LED Alarm Blinks Until Trap is Cleared)

01~FF (1~255 in Hours)
Values in the range 0 to 255 may be set.

The manufacturer defined default value is 0.

This parameter has the configuration ID ```config_5_1``` and is of type ```INTEGER```.


## Association Groups

Association groups allow the device to send unsolicited reports to the controller, or other devices in the network. Using association groups can allow you to eliminate polling, providing instant feedback of a device state change without unnecessary network traffic.

The DMMZ1 supports 4 association groups.

### Group 1: Group 1


This group supports 5 nodes.

### Group 2: Group 2


This group supports 5 nodes.

### Group 3: Group 3


This group supports 5 nodes.

### Group 4: Group 4


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
| COMMAND_CLASS_DEVICE_RESET_LOCALLY_V1| |
| COMMAND_CLASS_ZWAVEPLUS_INFO_V1| |
| COMMAND_CLASS_CONFIGURATION_V1| |
| COMMAND_CLASS_ALARM_V8| |
| COMMAND_CLASS_MANUFACTURER_SPECIFIC_V1| |
| COMMAND_CLASS_POWERLEVEL_V1| |
| COMMAND_CLASS_BATTERY_V1| |
| COMMAND_CLASS_WAKE_UP_V2| |
| COMMAND_CLASS_ASSOCIATION_V2| |
| COMMAND_CLASS_VERSION_V2| |

---

Did you spot an error in the above definition or want to improve the content?
You can [edit the database here](http://www.cd-jackson.com/index.php/zwave/zwave-device-database/zwave-device-list/devicesummary/684).
