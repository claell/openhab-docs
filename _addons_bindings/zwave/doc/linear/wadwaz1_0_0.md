---
layout: documentation
title: WADWAZ-1 - ZWave
---

{% include base.html %}

# WADWAZ-1 Door/Windows Sensor
This describes the Z-Wave device *WADWAZ-1*, manufactured by *Linear Corp* with the thing type UID of ```linear_wadwaz1_00_000```.

The device is in the category of Door, defining Door sensors.

# Overview

Linear Z-Wave products are easy to install, and allow dealers to create an integrated wireless network with nearly limitless expansion and interoperability with security and health monitoring systems, energy management, home entertainment, appliances, and more.

The WADWAZ-1 sensor monitors a door or window and sends Z-Wave signals when the door is opened or closed.

## Inclusion Information

Refer to your Controller operating instructions to add this module under the command of the Wireless Controller.

1. Unscrew the screw fastening the rear cover and slide the rear cover down.
2. Insert a CR123A battery into the battery compartment and LED will start to fl ash slowly, which means the sensor has not yet performed “inclusion” with the Controller.
3. Prepare the Controller to include a unit to the network by adding it to a group (method of adding a node to the network). Refer to the Controller instructions.
4. If your Controller supports Network Wide Inclusion (NWI) locate the WADWAZ-1 near the proposed installation location. If not skip to Step 6.
5. With your Controller in Inclusion mode, you should see an indication on your Controller that the “device was included” in the network. It should display binary switch / Linear. The LED will stop blinking. Skip to Step 9. If the LED does not stop blinking, relocate the WADWAZ-1 to within 100 feet (line of sight) of a Z-Wave device or your hub and repeat Step 5. If the LED continues to blink, your Controller does not support NWI and continue with Step 6.
6. Place the WADWAZ-1 within 3 feet of the Controller.
7. With your Controller in Inclusion mode, depress the Program switch for 1 second then release.
8. You should see an indication on your Controller that the “device was included” in the network. It should display binary switch / Linear. The LED will stop blinking.
9. The device will appear in the list of Switches

**NOTE**: If you have trouble adding the WADWAZ-1 to a group it may be that the Home ID and Node ID were not cleared from it after testing. You must first “RESET UNIT” with your Controller to remove it from the network. Although adding it to a group includes it in the network, removing it from a group does not remove it from the network. If removed from a group, it functions as a repeater (only). “RESET UNIT” removes it completely from the network

## Exclusion Information

For “Exclusion” from (removing from) a network:

1. Set up the Z-WaveTM Interface Controller into “exclusion” mode, and following its instruction to delete the WADWAZ-1 from the Controller.
2. Press the Program switch of WADWAZ-1 for 1 second and release to be excluded. The LED light will fl ash continuously when the sensor is in the Exclusion condition.

## Wakeup Information

Open and then closed the cover to wakeup the device. This will also trigger the tamper alarm, which needs to be turned off manually.

## Channels

The following table summarises the channels available for the WADWAZ-1

| Channel | Channel Id | Category | Item Type |
|---------|------------|----------|-----------|
| Sensor (Binary) | sensor_door | Door | Contact | 
| Sensor (Alarm) | alarm_entry | Door | Switch | 
| Tamper Alarm | alarm_tamper |  | Switch | 
| Sensor (External Switch) | sensor_binary | Door | Switch | 

### Sensor (Binary)

The ```sensor_door``` channel supports the ```Contact``` item and is in the ```Door``` category. This is a read only channel so will only be updated following state changes from the device.

The following state translation is provided for this channel to the ```Contact``` item type -:

| Value | Label     |
|-------|-----------|
| OPEN | Open |
| CLOSED | Closed |

### Sensor (Alarm)

The ```alarm_entry``` channel supports the ```Switch``` item and is in the ```Door``` category. This is a read only channel so will only be updated following state changes from the device.

The following state translation is provided for this channel to the ```Switch``` item type -:

| Value | Label     |
|-------|-----------|
| ON | Open |
| OFF | Closed |

### Tamper Alarm

The ```alarm_tamper``` channel supports the ```Switch``` item. This is a read only channel so will only be updated following state changes from the device.

The following state translation is provided for this channel to the ```Switch``` item type -:

| Value | Label     |
|-------|-----------|
| OFF | Ok |
| ON | Alarm |

### Sensor (External Switch)

The ```sensor_binary``` channel supports the ```Switch``` item and is in the ```Door``` category. This is a read only channel so will only be updated following state changes from the device.

The following state translation is provided for this channel to the ```Switch``` item type -:

| Value | Label     |
|-------|-----------|
| ON | Triggered |
| OFF | Untriggered |



## Device Configuration

The device has no configuration parameters configugured.

## Association Groups

Association groups allow the device to send unsolicited reports to the controller, or other devices in the network. Using association groups can allow you to eliminate polling, providing instant feedback of a device state change without unnecessary network traffic.

The WADWAZ-1 supports 1 association group.

### Group 1: Controller Updates


This group supports 5 nodes.

## Technical Information

### Endpoints

#### Endpoint 0

| Command Class | Comment |
|---------------|---------|
| COMMAND_CLASS_NO_OPERATION_V1| |
| COMMAND_CLASS_BASIC_V1| |
| COMMAND_CLASS_SENSOR_BINARY_V1| Linked to BASIC|
| COMMAND_CLASS_ALARM_V2| |
| COMMAND_CLASS_MANUFACTURER_SPECIFIC_V1| |
| COMMAND_CLASS_BATTERY_V1| |
| COMMAND_CLASS_WAKE_UP_V2| |
| COMMAND_CLASS_ASSOCIATION_V1| |
| COMMAND_CLASS_VERSION_V1| |

---

Did you spot an error in the above definition or want to improve the content?
You can [edit the database here](http://www.cd-jackson.com/index.php/zwave/zwave-device-database/zwave-device-list/devicesummary/9).
