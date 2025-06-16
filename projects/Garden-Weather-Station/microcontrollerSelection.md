# Microcontroller Selection

|Design Considerations|Team Project-Specific Requirements|Pic Option 1|Pic Option 2|Pic Option 3|
|-----------------------|------------------------------------|--------------|--------------|--------------|
|How many GPIO Pins?|10 would be preferable|Yes, 35|Yes, 25|Yes, 22|
|Built-in Analog to Digital Converter? How many?|We do not require any|Yes,10|Yes, 13|No|
|Built-in Hardware PWM? How many?|We need 1, but more than that would be optimal.|Yes, 5|Yes, 5|Yes, 2|
|Built-in I2C? SPI? How many?|We need 2|Both, 2 I2c, 4 SPI|Both, 2| SPI, 1|
|Built-in UART? How many?|We need 1|Yes, 2|Yes, 2|Yes, 1|
|Other Required Built-In Features? (optional)|-|-|-|-|
|Additional considerations specific to your project specifications (optional)|-|-|-|-|
||||||
|**Microcontroller Considerations**|**Team Project-Specific Requirements**|**Pic Option 1**|**Pic Option 2**|**Pic Option 3**|
|Part Number|Include the entire part number (leave off any letters at the end that specify the package type)|PIC18F46K22|PIC24FJ64GB004|ATMEGA16U2|
|Link (URL) to product page|Do not paste links directly into the table. Instead, [link them like this](http://www.microchip.com/).|[Digikey](https://www.digikey.com/en/products/detail/microchip-technology/PIC18F46K22-I%2FPT/2480377?utm_adgroup=General&utm_source=google&utm_medium=cpc&utm_campaign=PMax%20Shopping_Product_Zombie%20SKUs&utm_term=&utm_content=General&utm_id=go_cmp-17815035045_adg-_ad-__dev-c_ext-_prd-2480377_sig-CjwKCAiA8YyuBhBSEiwA5R3-E0WcTjmkh3ocqkXubYmM6NyJljwsgHKF0fGO5RUWoIMPZdxvoapPGhoC0_oQAvD_BwE&gad_source=1&gclid=CjwKCAiA8YyuBhBSEiwA5R3-E0WcTjmkh3ocqkXubYmM6NyJljwsgHKF0fGO5RUWoIMPZdxvoapPGhoC0_oQAvD_BwE)|[DigiKey](https://www.digikey.com/en/products/detail/microchip-technology/PIC24FJ64GB004T-I-PT/2178702)|[DigiKey](https://www.digikey.com/en/products/detail/microchip-technology/ATMEGA16U2-AU/2050947?utm_adgroup=&utm_source=google&utm_medium=cpc&utm_campaign=PMax%20Shopping_Product_Medium%20ROAS%20Categories&utm_term=&utm_content=&utm_id=go_cmp-20223376311_adg-_ad-__dev-c_ext-_prd-2050947_sig-CjwKCAiA_OetBhAtEiwAPTeQZylS3Tnj3xmcfaoHoJbeJCH6C-Cq70qy1CSXnq_WX1M5NZ4RLNCOmRoC2joQAvD_BwE&gad_source=1&gclid=CjwKCAiA_OetBhAtEiwAPTeQZylS3Tnj3xmcfaoHoJbeJCH6C-Cq70qy1CSXnq_WX1M5NZ4RLNCOmRoC2joQAvD_BwE)|
|Links (URL) to Data Sheets|See #4|[DataSheet](https://ww1.microchip.com/downloads/en/DeviceDoc/PIC18(L)F2X-4XK22-Data-Sheet-40001412H.pdf)|[DataSheet](https://ww1.microchip.com/downloads/en/DeviceDoc/39940d.pdf)|[DataSheet](https://ww1.microchip.com/downloads/en/DeviceDoc/7799S.pdf)|
|Links (URL) to Application Notes|Often provided by manufacturers to give you specific examples of how to use their products. Search for them in the search bar on the Microchip’s website.|[Scroll down](https://www.microchip.com/en-us/product/PIC18F46K22)|[Scroll Down](https://www.microchip.com/en-us/product/PIC24FJ64GB004)|[Scroll Down](https://www.microchip.com/en-us/product/ATmega16U2)|
|Links (URL) to Code Examples||[MicroChip](https://www.microchip.com/en-us/code-examples) [ASC ICC](https://embedded-systems-design.bitbucket.io/314/314-icc-05-pic-advanced-serial-communication/)|[MicroChip](https://www.microchip.com/en-us/code-examples) [ASC ICC](https://embedded-systems-design.bitbucket.io/314/314-icc-05-pic-advanced-serial-communication/)|[MicroChip](https://www.microchip.com/en-us/code-examples) [ASC ICC](https://embedded-systems-design.bitbucket.io/314/314-icc-05-pic-advanced-serial-communication/)|
|Links (URL) to External Resources|Search on Google and YouTube for other resources for each specific microcontroller.|[MPLAB Tutorial](https://www.youtube.com/playlist?list=PL_zvrXFdKgZpTrM99mypGVW5JBZ6tQZiR)|[MPLAB Tutorial](https://www.youtube.com/playlist?list=PL_zvrXFdKgZpTrM99mypGVW5JBZ6tQZiR)|[MPLAB Tutorial](https://www.youtube.com/playlist?list=PL_zvrXFdKgZpTrM99mypGVW5JBZ6tQZiR)|
|Production Unit Cost|Find in the Microchip online store, or Digikey|$3.89|$5.10|$3.24|
|Supply Voltage Range|Find in the microcontroller datasheet|2.3-5.5V|2.0-3.6V|2.7-5.5V|
|Absolute Maximum Current for entire IC|Find in the microcontroller datasheet|200 mA|200 mA|200 mA|
|Maximum GPIO Pin Current (Source/Sink)|Find in the microcontroller datasheet|25 mA|25 mA|40 mA|
|8-bit or 16-bit Architecture|Find in the microcontroller datasheet|8-bit|16-bit|8-bit|
|Available IC Packages / Footprints|Find in the microcontroller datasheet. Choose a microcontroller with both surface mount and DIP/through-hole packages available. See Most Common Mistakes below for requirements to improve manufacturing reliability.|TQFP <br> QFN <br> VQFN <br> UQFN <br> PDIP <br> SSOP <br> SOIC <br> SPDIP <br>|TQFP <br> QFN <br> SSOP <br> SOIC <br> SPDIP <br>|TQFP <br> QFN <br>|
|Supports External Interrupts?|Find in the microcontroller datasheet|Yes|Yes|Yes|
|In-System Programming Capability and Type|Allows for programming the microcontroller without removing it from the PCB. Find in the microcontroller datasheet.|Yes, ICSP|Yes, ICSP|Yes, debugWIRE|
|Programming Hardware, Cost, and URL|Find on the microcontroller product page|[PiCKit 5](https://www.microchip.com/en-us/development-tool/PG164150) $94.99|[PiCKit 5](https://www.microchip.com/en-us/development-tool/PG164150) <br> $94.99|[PiCKit 5](https://www.microchip.com/en-us/development-tool/PG164150) $94.99|
|Works with [MPLAB® X Integrated Development Environment](https://www.microchip.com/mplab/mplab-x-ide) (IDE)|Required. See [Microchip Development Tools](https://www.microchip.com/development-tools)|Yes|Yes|Yes|
|Works with [Microchip Code Configurator](https://www.microchip.com/mplab/mplab-code-configurator)?|Required. Go to the [MCC website](https://www.microchip.com/en-us/tools-resources/configure/mplab-code-configurator), click the “Manual Downloads” tab, scroll to the device library that goes with the PIC you chose (likely “MCC 8-bit PIC”) and read the release notes to make sure your microcontroller is in the list of supported devices.|Yes|Yes|Yes|
||||||
|Overall Pros|Write at least 2 for each microcontroller|Has two channels for I2C and SPI <br> <br> Lots of GPIO pins for possible additional features (LCD, etc.) <br> <br> Wide-ranging supply voltage TQFP is the best option as other package sizes (which are bigger) are hard to get a hold of. <br> <br>  Similar to the MC’s we have already been using|Low Power Consumption <br> <br> Lots of ADC channels|High performance with a low power output/draw <br> <br> Lots of memory, which is good for a complex project like this|
|Overall Cons|Write at least 2 for each microcontroller|Lots of pins, and comes in a TQFP package size, making it hard to solder <br> <br> Lots of unused pins|Possibly really hard to solder, as it might require baking <br> <br> Possibly too many features creating a steep learning curve|No I2C Pins <br> <br> Limited Analog features (no ADC)|
|Ranking|1 = first <br> 2 = second <br> 3 = third|1|2|3|

<br>

**Final Microcontroller Choice:** Option 1: PIC18F46K22

<br>

**Rationale:** This microcontroller meets all of our needs and seems to be the easiest to work with in terms of programming and soldering
<!--stackedit_data:
eyJoaXN0b3J5IjpbNTM5MDA3MDg4XX0=
-->
