# Arduino-Mega Compatible Secure Connectivity Development Platform

**WARNING**: This project is under development and has not yet been validated.

This is an open hardware platform designed for the development of secure wired-network applications. It is fully compatible with all Arduino Mega-compatible hardware and software.

This project was inspired by (but not a copy of) the Freetronics EtherMega: https://github.com/freetronics/EtherMega
This project was created as an alternative to the platform offered by Freetronics.

Features:
- CH340 USB->Serial Converter (Functionally similar to FT232, Driver should be installed automatically)
- Jumper Configurable IO: Certain pins (D3, D6, D8, D9, D13) can be connected to the headers or to integrated peripheral pins.
- 5V 2A USB-C Input
- 6V - 32V VIN Input 
- MicroSD Card Slot
- 10/100 Ethernet provided over SPI using the W6100. Supports Auto-Negotiations, IPv4, IPv6, and Auto-MIDX.
- SE050 EdgeLock Plug and Trust Secure Element to provide security features for connected applications, accessible using I2C
- ISM330DHCX Inertial Measurement Unit, accessible using I2C
- MCP7940N Real Time Clock, accessible using I2C
- Level Shifted I2C: Provides connection points for 3V3 I2C Devices (Extra Header), and 5V I2C Devices (Standard Mega Headers)
  

## Top Render
![Render of Top of PCB](https://github.com/dmanla/ArduinoMegaEthernet/blob/main/3D_Render_TOP.JPG)

## Bottom Render
![Render of Bottom of PCB](https://github.com/dmanla/ArduinoMegaEthernet/blob/main/3D_Render_BOTTOM.JPG)

## Side Render
![Render of Side of PCB](https://github.com/dmanla/ArduinoMegaEthernet/blob/main/3D_Render_ANGLED.JPG)

## Relevant Datasheets

- [CH340N](https://datasheet.lcsc.com/szlcsc/Jiangsu-Qin-Heng-CH340C_C84681.pdf): USB->Serial Bridge
- [AP22805AW5](https://www.diodes.com/assets/Datasheets/AP22804_14.pdf): USB Protection
- [AP63205](https://www.diodes.com/assets/Datasheets/AP63200-AP63201-AP63203-AP63205.pdf): DC-DC Switching Converters
- [W5500](http://wizwiki.net/wiki/lib/exe/fetch.php/products:w5500:w5500_ds_v109e.pdf): SPI->Ethernet Bridge
- [ISM330DHCX](https://www.st.com/resource/en/datasheet/ism330dhcx.pdf): "AI Enabled" Inertial Measurement Unit
- [SE050C2HQ1](https://www.nxp.com/docs/en/data-sheet/SE050-DATASHEET.pdf): Security Coprocessor
- [MCP7940N](http://ww1.microchip.com/downloads/en/DeviceDoc/20005010F.pdf): Real-Time Clock **with** Battery Backup
- [Atmega2560](http://ww1.microchip.com/downloads/en/DeviceDoc/Atmel-2549-8-bit-AVR-Microcontroller-ATmega640-1280-1281-2560-2561_datasheet.pdf): Main Microcontroller

