# [Tested Zigbee devices](https://github.com/smlight-tech/slzb-os-zigbee-hub/tree/main/devices_support)

# What is the operating mode: Zigbee Hub?
<img src="./images/regular_tcp.jpg?raw=true" width=650px/><br>
The normal TCP bridge mode forwards raw ZigBee traffic over the network to be processed by Z2M or ZHA. This means that you are highly dependent on network stability and any packet loss will lead to errors.<br>
The advantages of this solution are that you have high CPU processing power for ZigBee traffic since Z2M/ZHA is running on a PC.

<img src="./images/zb_hub.jpg?raw=true" width=650px/><br>
Zigbee Hub is a mode that provides processing of all Zigbee traffic within the SLZB-OS system **without the need to use ZHA or Z2M**.<br>
This provides excellent stability, since now there is no need to send raw Zigbee packets over the network, but instead ready-processed messages are sent.<br>
The loss of a ready message will **not lead to a failure in the hub** (as happens with ZHA/Z2M).<br>
MQTT integration allows you to ensure traffic integrity (with QOS > 0).<br>
The disadvantage of this solution is the limited CPU power of the SLZB-06 controller, which leads to a limitation of the maximum number of ZigBee devices that it can process.<br>
Also, the support for the functionality of ZigBee devices is limited (will be expanded over time)

# **Zigbee chip update warning**
Currently, Zigbee Hub does not support restoring a backup of your Zigbee network after a Zigbee chip firmware update!<br>
This means that after updating the Zigbee chip firmware, you will have to **re-pair all your Zigbee devices!**

# What is currently supported?
## Power config cluster (0x0001)
- Battery charge (for battery-powered devices)

This cluster binds automatically.

## IAS Zone (0x0500)
- Door opening sensors
- Motion sensors
- Vibration sensors
- Glass breakage sensors

Alarm1 or Alarm2 is considered as a trigger.

## On/Off (0x0006)
- On/Off (current switch state)
- On/Off command (switch control)

This cluster binds automatically.

## Temperature Measurement (0x0402)
- MeasuredValue (current temperature)

This cluster binds automatically.

## Pressure Measurement (0x0403)
- MeasuredValue (current pressure)

This cluster binds automatically.

## Flow Measurement (0x0404) (Testing is needed!)
- MeasuredValue (current flow)

This cluster binds automatically.

## Relative Humidity Measurement (0x0405)
- MeasuredValue (current humidity)

This cluster binds automatically.

## Electrical Measurement (0x0b04)
- RMSVoltage
- RMSCurrent
- ActivePower

This cluster does not bind automatically!<br>
The system will try to determine the voltage divider on its own.<br>
Current divider - 10000<br>
Power divider - 1<br>