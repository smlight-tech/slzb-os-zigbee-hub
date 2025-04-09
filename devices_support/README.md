# Below you can find a list with information about ZigBee devices support

| Manufacturer  | Device Model  | Device Link    | What Works                                | What Doesn't Work   | Notes         |
| ------------- | ------------- | -------------  | -------------                             | -------------       | ------------- |
| eWeLink       | SNZB-02P      |                | Temperature<br>Humidity<br>Battery charge |                     |               |
| eWeLink  | MS01  |                |Battery charge<br>Motion detection|                     |                     | |
|_TZ3000_abci1hiu|TS0044| | |Button commands are currently not sent via MQTT.<br>Battery level is not detected correctly.<br>Drains battery quickly.|Expose 4 clusters ON/OFF|
|_TZ3000_wzmuk9ai|TS011F| |ON/OFF|Does not support voltage, current, and power reporting|Requires development of pooling functionality|
|_TZ3000_8yhypbo7|TS0203| |Battery charge<br>Door status (closed/open)| | |
|_TZ3000_itnrsufe|TS0201| |Temperature<br>Humidity<br>Battery charge| |Drains battery quickly|
|LUMI|lumi.weather| |Temperature<br>Humidity<br>Pressure|Battery charge| |
|eWeLink|CK-BL702-AL-01(7009_Z102LG03-1)| |ON/OFF|Brightness<br>Color<br>Touchlink|Requires support for clusters 0x0300, 0x0008|
|_TZ3000_kqvb5akv|TS0001| |ON/OFF<br>Voltage<br>Crrent<br>Power| | |
|_TZ3000_abrsvsou|TS004F| |Battery|Button commands are currently not sent via MQTT| | |