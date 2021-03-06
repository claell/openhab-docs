---
layout: documentation
title: DTHERMZ5 - ZWave
---

{% include base.html %}

# DTHERMZ5 Z-Wave room sensor
This describes the Z-Wave device *DTHERMZ5*, manufactured by *Danfoss* with the thing type UID of ```danfoss_dthermz5_00_000```.

# Overview


## Channels

The following table summarises the channels available for the DTHERMZ5

| Channel | Channel Id | Category | Item Type |
|---------|------------|----------|-----------|
| Sensor (temperature) | sensor_temperature | Temperature | Number | 
| Setpoint (cooling) | thermostat_setpoint | Temperature | Number | 
| Setpoint (heating) | thermostat_setpoint | Temperature | Number | 
| Scene Number | scene_number |  | Number | 

### Sensor (temperature)

The ```sensor_temperature``` channel supports the ```Number``` item and is in the ```Temperature``` category. This is a read only channel so will only be updated following state changes from the device.

### Setpoint (cooling)

The ```thermostat_setpoint``` channel supports the ```Number``` item and is in the ```Temperature``` category.

### Setpoint (heating)

The ```thermostat_setpoint``` channel supports the ```Number``` item and is in the ```Temperature``` category.

### Scene Number

The ```scene_number``` channel supports the ```Number``` item.



## Device Configuration

The following table provides a summary of the 11 configuration parameters available in the DTHERMZ5.
Detailed information on each parameter can be found in the sections below.

| Param | Name  | Description |
|-------|-------|-------------|
| 1 | Temperature Report threshold | Range is from 0.1 to 10°C 1=0.1°C 100=10°C |
| 2 | Set-point display resolution | range from 0.1 to 10°C 1=0.1°C 100=10°C |
| 3 | Min Set-point and override limit | from min 0°C to max setpoint override limit 0=0°C 40=40°C |
| 4 | Max Set-point and override limit | from min setpoint override limit to max 40°C 0=0°C 40=40°C |
| 5 | LED Flash period | 0 to 65535 seconds |
| 6 | Set-point control function | 0=Disabled 1=Enabled |
| 7 | Temporarily override scheduler | 0=Disabled 1=Enabled |
| 8 | Set-point type in Thermostat_Setpoint_Reports | 1=Heating 2=Cooling 10=Auto Changeover |
| 9 | LED on time | 1=100ms 5=500ms |
| 10 | Number of LED flashes (duration) | 0 to 255 |
| 11 | LED color | 1=Green 2=Red |

### Parameter 1: Temperature Report threshold

Range is from 0.1 to 10°C 1=0.1°C 100=10°C
Default value 5 = 0.5 °C
Values in the range 1 to 100 may be set.

The manufacturer defined default value is 5.

This parameter has the configuration ID ```config_1_2``` and is of type ```INTEGER```.


### Parameter 2: Set-point display resolution

range from 0.1 to 10°C 1=0.1°C 100=10°C

Values in the range 1 to 100 may be set.

The manufacturer defined default value is 5.

This parameter has the configuration ID ```config_2_2``` and is of type ```INTEGER```.


### Parameter 3: Min Set-point and override limit

from min 0°C to max setpoint override limit 0=0°C 40=40°C

Values in the range 0 to 40 may be set.

The manufacturer defined default value is 12.

This parameter has the configuration ID ```config_3_2``` and is of type ```INTEGER```.


### Parameter 4: Max Set-point and override limit

from min setpoint override limit to max 40°C 0=0°C 40=40°C

Values in the range 0 to 40 may be set.

The manufacturer defined default value is 28.

This parameter has the configuration ID ```config_4_2``` and is of type ```INTEGER```.


### Parameter 5: LED Flash period

0 to 65535 seconds

Values in the range 0 to 65535 may be set.

The manufacturer defined default value is 1.

This parameter has the configuration ID ```config_5_4``` and is of type ```INTEGER```.


### Parameter 6: Set-point control function

0=Disabled 1=Enabled

The following option values may be configured -:

| Value  | Description |
|--------|-------------|
| 0 | disabled |
| 1 | enabled |

The manufacturer defined default value is 1 (enabled).

This parameter has the configuration ID ```config_6_1``` and is of type ```INTEGER```.


### Parameter 7: Temporarily override scheduler

0=Disabled 1=Enabled

The following option values may be configured -:

| Value  | Description |
|--------|-------------|
| 0 | disabled |
| 1 | enabled |

The manufacturer defined default value is 1 (enabled).

This parameter has the configuration ID ```config_7_1``` and is of type ```INTEGER```.


### Parameter 8: Set-point type in Thermostat_Setpoint_Reports

1=Heating 2=Cooling 10=Auto Changeover

The following option values may be configured -:

| Value  | Description |
|--------|-------------|
| 1 | Heating |
| 2 | Cooling |
| 10 | Auto-Changeover |

The manufacturer defined default value is 1 (Heating).

This parameter has the configuration ID ```config_8_1``` and is of type ```INTEGER```.


### Parameter 9: LED on time

1=100ms 5=500ms

Values in the range 1 to 5 may be set.

The manufacturer defined default value is 1.

This parameter has the configuration ID ```config_9_2``` and is of type ```INTEGER```.


### Parameter 10: Number of LED flashes (duration)

0 to 255

Values in the range 0 to 255 may be set.

The manufacturer defined default value is 5.

This parameter has the configuration ID ```config_10_1``` and is of type ```INTEGER```.


### Parameter 11: LED color

1=Green 2=Red

The following option values may be configured -:

| Value  | Description |
|--------|-------------|
| 1 | Green |
| 2 | Red |

The manufacturer defined default value is 1 (Green).

This parameter has the configuration ID ```config_11_1``` and is of type ```INTEGER```.


## Association Groups

Association groups allow the device to send unsolicited reports to the controller, or other devices in the network. Using association groups can allow you to eliminate polling, providing instant feedback of a device state change without unnecessary network traffic.

The device does not support associations.
## Technical Information

### Endpoints

#### Endpoint 0

| Command Class | Comment |
|---------------|---------|
| COMMAND_CLASS_NO_OPERATION_V1| |
| COMMAND_CLASS_BASIC_V1| |
| COMMAND_CLASS_SENSOR_MULTILEVEL_V6| |
| COMMAND_CLASS_THERMOSTAT_SETPOINT_V1| |
| COMMAND_CLASS_SCHEDULE_V1| |
| COMMAND_CLASS_CENTRAL_SCENE_V1| |
| COMMAND_CLASS_CONFIGURATION_V1| |
| COMMAND_CLASS_MANUFACTURER_SPECIFIC_V1| |
| COMMAND_CLASS_PROTECTION_V2| |
| COMMAND_CLASS_BATTERY_V1| |
| COMMAND_CLASS_WAKE_UP_V2| |
| COMMAND_CLASS_VERSION_V2| |
| COMMAND_CLASS_INDICATOR_V1| |
| COMMAND_CLASS_MULTI_CMD_V1| |

---

Did you spot an error in the above definition or want to improve the content?
You can [edit the database here](http://www.cd-jackson.com/index.php/zwave/zwave-device-database/zwave-device-list/devicesummary/501).
