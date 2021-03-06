---
layout: documentation
title: HTP-4S1-FB - ZWave
---

{% include base.html %}

# HTP-4S1-FB Four Touch Panel and Power Socket
This describes the Z-Wave device *HTP-4S1-FB*, manufactured by *Hogar Controls* with the thing type UID of ```hogar_htp4s1fb_02_002```.
This version of the device is limited to firmware versions above 2.2

# Overview

The HOGAR Touch Panels features a stunning glass face with advanced capacitive touch sensor engineered with smart home wireless standards Zigbee, Z-Wave Plus and Wifi variants.

The Smart Home deserves better than an ordinary light switch. Hogar touch panels are one-of-a-kind collection of switches, dimmers, and scene controller that will transform walls from boring to absolutely breath-taking.

Fits in existing electrical box and does not require new wires. Innovative assembly and snap-in system make it fast and simple to install.

Please visit http://hogarcontrols.com/shop/touch-panels/four-touch-panel-socket for more information.

## Inclusion Information

1\. Tap and hold any of the touch button for few seconds (about 7 seconds).

2\. The LEDs of all the buttons will turn solid red all at the same time.

3\. At that time, release the button and tap it again only once.

4\. The LED of the button will flash pink (once) indicating that the device is ready to be included.

## Exclusion Information

1\. Tap and hold any of the touch button for few seconds (about 7 seconds).

2\. The LEDs of all the buttons will turn solid red all at the same time.

3\. At that time, release the button and tap it again only once.

4\. The LED of the button will flash pink (once) indicating that the device is ready to be included.

## Channels

The following table summarises the channels available for the HTP-4S1-FB

| Channel | Channel Id | Category | Item Type |
|---------|------------|----------|-----------|
| Switch | switch_binary | Switch | Switch | 
| Switch 1 | switch_binary1 | Switch | Switch | 
| Switch 2 | switch_binary2 | Switch | Switch | 
| Switch 3 | switch_binary3 | Switch | Switch | 
| Switch 4 | switch_binary4 | Switch | Switch | 

### Switch

The ```switch_binary``` channel supports the ```Switch``` item and is in the ```Switch``` category.

### Switch 1

The ```switch_binary1``` channel supports the ```Switch``` item and is in the ```Switch``` category.

### Switch 2

The ```switch_binary2``` channel supports the ```Switch``` item and is in the ```Switch``` category.

### Switch 3

The ```switch_binary3``` channel supports the ```Switch``` item and is in the ```Switch``` category.

### Switch 4

The ```switch_binary4``` channel supports the ```Switch``` item and is in the ```Switch``` category.



## Device Configuration

The device has no configuration parameters configugured.

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
| COMMAND_CLASS_SWITCH_BINARY_V1| Linked to BASIC|
| COMMAND_CLASS_SWITCH_ALL_V1| |
| COMMAND_CLASS_MULTI_CHANNEL_V1| |
| COMMAND_CLASS_CONFIGURATION_V1| |
| COMMAND_CLASS_MANUFACTURER_SPECIFIC_V1| |
| COMMAND_CLASS_ASSOCIATION_V1| |
| COMMAND_CLASS_VERSION_V1| |
#### Endpoint 1

| Command Class | Comment |
|---------------|---------|
| COMMAND_CLASS_BASIC_V1| |
| COMMAND_CLASS_SWITCH_BINARY_V1| Linked to BASIC|
#### Endpoint 2

| Command Class | Comment |
|---------------|---------|
| COMMAND_CLASS_NO_OPERATION_V1| |
| COMMAND_CLASS_BASIC_V1| |
| COMMAND_CLASS_SWITCH_BINARY_V1| Linked to BASIC|
#### Endpoint 3

| Command Class | Comment |
|---------------|---------|
| COMMAND_CLASS_BASIC_V1| |
| COMMAND_CLASS_SWITCH_BINARY_V1| Linked to BASIC|
#### Endpoint 4

| Command Class | Comment |
|---------------|---------|
| COMMAND_CLASS_BASIC_V1| |
| COMMAND_CLASS_SWITCH_BINARY_V0| Linked to BASIC|

---

Did you spot an error in the above definition or want to improve the content?
You can [edit the database here](http://www.cd-jackson.com/index.php/zwave/zwave-device-database/zwave-device-list/devicesummary/545).
