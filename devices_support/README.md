# Below you can find a list with information about ZigBee devices support

|Image | Manufacturer  | Device Model  | Device Link    | What Works                                | What Doesn't Work   | Notes         |
| - | ------------- | ------------- | -------------  | -------------                             | -------------       | ------------- |
|<img src="./images/eWeLink.SNZB-02P.jpg?raw=true" width=100px/>| eWeLink       | SNZB-02P      |                | Temperature<br>Humidity<br>Battery |                     |               |
|<img src="./images/eWeLink.MS01.png?raw=true" width=100px/>| eWeLink  | MS01  |                |Battery<br>Motion detection|                     |                     | |
|<img src="./images/_TZ3000_abci1hiu.TS0044.webp?raw=true" width=100px/>|_TZ3000_abci1hiu|TS0044| | |Button commands are currently not sent via MQTT.<br>Battery level is not detected correctly|Expose 4 clusters ON/OFF<br>Drains battery quickly|
|<img src="./images/_TZ3000_wzmuk9ai.TS011F.png?raw=true" width=100px/>|_TZ3000_wzmuk9ai|TS011F| |ON/OFF|Does not support voltage, current, and power reporting|Requires development of pooling functionality|
|<img src="./images/_TZ3000_8yhypbo7.TS0203.png?raw=true" width=100px/>|_TZ3000_8yhypbo7|TS0203| |Battery<br>Door status (closed/open)| | |
|<img src="./images/_TZ3000_itnrsufe.TS0201.png?raw=true" width=100px/>|_TZ3000_itnrsufe|TS0201| |Temperature<br>Humidity<br>Battery| |Drains battery quickly|
|<img src="./images/LUMI.lumi.weather.webp?raw=true" width=100px/>|LUMI|lumi.weather|https://www.aliexpress.com/item/1005007471041068.html|Temperature<br>Humidity<br>Pressure|Battery| |
|<img src="./images/eWeLink.CK-BL702-AL-01(7009_Z102LG03-1).png?raw=true" width=100px/>|eWeLink|CK-BL702-AL-01(7009_Z102LG03-1)|https://www.aliexpress.com/item/1005007183053442.html|ON/OFF<br>Brightness<br>Color<br>Color temperature|Touchlink||
|<img src="./images/_TZ3000_kqvb5akv.TS0001.png?raw=true" width=100px/>|_TZ3000_kqvb5akv|TS0001| |ON/OFF<br>Voltage<br>Crrent<br>Power| | |
|<img src="./images/_TZ3000_abrsvsou.TS004F.png?raw=true" width=100px/>|_TZ3000_abrsvsou|TS004F|https://www.aliexpress.com/item/1005007475312050.html|Battery|Button commands are currently not sent via MQTT| | |
|<img src="./images/_TZE204_d7lpruvi.TS0601.png?raw=true" width=100px/>|_TZ3000_abrsvsou|TS004F|https://www.aliexpress.com/item/1005006861229185.html|Date/Time sync|Temperature<br>Humidity<br>Battery|Requires SLZB-OS v2.8.8 or higher|