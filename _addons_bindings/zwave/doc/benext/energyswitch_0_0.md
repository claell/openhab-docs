---
layout: documentation
title: Energy Switch + - ZWave
---

{% include base.html %}

# Energy Switch + Energy Switch +
This describes the Z-Wave device *Energy Switch +*, manufactured by *BeNext* with the thing type UID of ```benext_energyswitch_00_000```.

# Overview


## Channels

The following table summarises the channels available for the Energy Switch +

| Channel | Channel Id | Category | Item Type |
|---------|------------|----------|-----------|
| Switch | switch_binary | Switch | Switch | 
| Electric meter (kWh) | meter_kwh | Energy | Number | 
| Electric meter (watts) | meter_watts | Energy | Number | 

### Switch

The ```switch_binary``` channel supports the ```Switch``` item and is in the ```Switch``` category.

### Electric meter (kWh)

The ```meter_kwh``` channel supports the ```Number``` item and is in the ```Energy``` category. This is a read only channel so will only be updated following state changes from the device.

### Electric meter (watts)

The ```meter_watts``` channel supports the ```Number``` item and is in the ```Energy``` category. This is a read only channel so will only be updated following state changes from the device.



## Device Configuration

The following table provides a summary of the 9 configuration parameters available in the Energy Switch +.
Detailed information on each parameter can be found in the sections below.

| Param | Name  | Description |
|-------|-------|-------------|
| 1 | Set to Default | If value is set to 0XFF (255), device set to default |
| 2 | Amount of decimals | If value is set to 1 the info shall be presented with 1 decimal |
| 3 | Power Limit  | The device will shut down when it reaches an amount higher then defined (W) |
| 4 | Start up with last known socket status | If 0 then the device will always be off, when 1-255 it will emain the last known state |
| 6 | Auto report % | The value will change when the % is changed. |
| 7 | Auto report Watt | The value will change when the Watt is changed. |
| 8 | Auto report time | The time between 2 of the meter rerport |
| 9 | Relais delay time | The time that needs to pass before the next state change |
| 10 | Led indicator | The state of the Led compared to the relais state |

### Parameter 1: Set to Default

If value is set to 0XFF (255), device set to default

Values in the range 0 to 255 may be set.

The manufacturer defined default value is 0.

This parameter has the configuration ID ```config_1_1``` and is of type ```INTEGER```.


### Parameter 2: Amount of decimals

If value is set to 1 the info shall be presented with 1 decimal
0,1,2,3 amount of decimals. Every Amount higher then 3 shall be printed as 3 decimals.
Values in the range 0 to 3 may be set.

The manufacturer defined default value is 0.

This parameter has the configuration ID ```config_2_1``` and is of type ```INTEGER```.


### Parameter 3: Power Limit 

The device will shut down when it reaches an amount higher then defined (W)
0 = no power limit.

1-4500 are acceptable values and can be used, everything above the 4500 shall be changed to 4500.
Values in the range 0 to 4500 may be set.

The manufacturer defined default value is 4500.

This parameter has the configuration ID ```config_3_2``` and is of type ```INTEGER```.


### Parameter 4: Start up with last known socket status

If 0 then the device will always be off, when 1-255 it will emain the last known state

Values in the range 0 to 255 may be set.

The manufacturer defined default value is 0.

This parameter has the configuration ID ```config_4_1``` and is of type ```INTEGER```.


### Parameter 6: Auto report %

The value will change when the % is changed.

Values in the range 10 to 100 may be set.

The manufacturer defined default value is 20.

This parameter has the configuration ID ```config_6_1``` and is of type ```INTEGER```.


### Parameter 7: Auto report Watt

The value will change when the Watt is changed.

Values in the range 5 to 255 may be set.

The manufacturer defined default value is 10.

This parameter has the configuration ID ```config_7_1``` and is of type ```INTEGER```.


### Parameter 8: Auto report time

The time between 2 of the meter rerport

Values in the range 10 to 255 may be set.

The manufacturer defined default value is 20.

This parameter has the configuration ID ```config_8_1``` and is of type ```INTEGER```.


### Parameter 9: Relais delay time

The time that needs to pass before the next state change
Value \* 10 miliseconds
Values in the range 0 to 255 may be set.

The manufacturer defined default value is 50.

This parameter has the configuration ID ```config_9_1``` and is of type ```INTEGER```.


### Parameter 10: Led indicator

The state of the Led compared to the relais state
0 = Indication Led never off

1 = led ON when relais ON

2 = led On when relais OFF
Values in the range 0 to 2 may be set.

The manufacturer defined default value is 0.

This parameter has the configuration ID ```config_10_1``` and is of type ```INTEGER```.


## Association Groups

Association groups allow the device to send unsolicited reports to the controller, or other devices in the network. Using association groups can allow you to eliminate polling, providing instant feedback of a device state change without unnecessary network traffic.

The device does not support associations.
## Technical Information

### Endpoints

#### Endpoint 0

| Command Class | Comment |
|---------------|---------|
| COMMAND_CLASS_SWITCH_BINARY_V1| |
| COMMAND_CLASS_SWITCH_ALL_V1| |
| COMMAND_CLASS_METER_V3| |
| COMMAND_CLASS_CRC_16_ENCAP_V1| |
| COMMAND_CLASS_CONFIGURATION_V1| |
| COMMAND_CLASS_MANUFACTURER_SPECIFIC_V1| |
| COMMAND_CLASS_POWERLEVEL_V1| |
| COMMAND_CLASS_PROTECTION_V1| |
| COMMAND_CLASS_ASSOCIATION_V1| |
| COMMAND_CLASS_VERSION_V1| |

---

Did you spot an error in the above definition or want to improve the content?
You can [edit the database here](http://www.cd-jackson.com/index.php/zwave/zwave-device-database/zwave-device-list/devicesummary/445).
