# ESP32-C3-DevBoard
ESP32-C3 Development Board. This project uses [KiCAD](https://KiCAD.org)

You can get ESP32-C3-WROOM-02 from here.  
* [秋月電子](https://akizukidenshi.com/catalog/g/gM-17493/)  
* [DigiKey](https://www.digikey.jp/ja/products/detail/espressif-systems/ESP32-C3-WROOM-02-N4/14553031)
* [Mouser](https://www.mouser.jp/ProductDetail/Espressif-Systems/ESP32-C3-WROOM-02-N4?qs=stqOd1AaK7%2FqjTZKEOgfUg%3D%3D)

Orders can be placed by uploading data(gerber, bom, and cpl) to the JLCPCB. (Take note that ESP32-C3-WROOM-02 is not assembled for Economic PCBA.)  
This project uses [Espressif Library for KiCAD](https://github.com/espressif/kicad-libraries). (It is available on Plugin & Contents manager.)  
Gerber, bom and cpl is placed on [production folder](/production) directory and Release. 

## Features
* Upload method: USB-CDC (Do not use GPIO 18 and 19 when downloading)
* USB: Type-C
* Regulator: [RT9080-33GJ5](https://www.richtek.com/Products/Linear%20Regulator/Single%20Output%20Linear%20Regulator/RT9080?sc_lang=en).
* External input voltage range: ~6.5V (~5.5V is recommended)
* Power consumption (in deep sleep): 7~9µF (ESP32-C3: 5µF, RT9080-33GJ5: 2~4µF)

### Solder Jumpers
* 5V -> 3.3V jumper (Default: connected): Connection of the external power supply terminal (5 V pin) to the power input terminal to the ESP32-C3. Disconnect when suppressing regulator quiescent current.
* VBUS = 5V jumper (Default: not connected): Connecting this disables the protective SBD between USB and external power supply. To eliminate the voltage drop due to SBD and output the voltage input from USB as it is to 5 V, connect this jumper.

## BOM
[BOM](/production/bom.csv)

## 3D image
![image](/ESP32-C3-DevBoard.png)
