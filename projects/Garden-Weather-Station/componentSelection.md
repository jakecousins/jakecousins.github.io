# Component Selection
Component selection is an integral aspect of the engineering design process, as it significantly impacts future design and device development. As a team, we have developed a page dedicated to outlining the components selected for key subsystems, including power management and microcontroller integration, humidity and temperature sensing, and motor driver functionality. Below, you will find the chosen components, along with detailed explanations justifying their selection.

## [Temperature Sensor](https://www.digikey.com/en/products/detail/microchip-technology/TC74A4-3-3VCTTR/443268)
<img src="https://mm.digikey.com/Volume0/opasdata/d220001/medias/images/2386/150%7EC04-091%7ECT%2C%20OT%7E5.JPG" width="400" height="400">

After researching various temperature sensors that we could use we decided on the TC74A4-3.3VCTTR from Microchip Technology. This is a simple temperature sensor that fits our project perfectly. 

 - It uses the I2C communication protocol to interface with out micro controller which is required for this project. 
 - Has low power consumption
 - Uses 3.3V, this helps our design as are aiming for a very low voltage design
 - It has a wide range of temperatures it can capture

All of these factors fit very well into our design and thus we ultimately chose this temperature sensor over other competitors.

<br>

<br>

## [Humidity Sensor](https://www.digikey.com/en/products/detail/texas-instruments/HDC1080DMBT/5878615?utm_adgroup=Texas%20Instruments&utm_source=google&utm_medium=cpc&utm_campaign=PMax%20Shopping_Supplier_Texas%20Instruments&utm_term=&utm_content=Texas%20Instruments&utm_id=go_cmp-17816159938_adg-_ad-__dev-c_ext-_prd-5878615_sig-CjwKCAiAtt2tBhBDEiwALZuhAH7JbYuHTQ2nVUpdfYoOB3d2jpY02UwiI9HFjxSbYURg3e6y1LMyfhoCadcQAvD_BwE&gad_source=1)
<img src="https://mm.digikey.com/Volume0/opasdata/d220001/medias/images/1001/MFG_HDC1080DMBR.jpg" width="400" height="400">

The Texas Instruments HDC1080DMBT is a fantastic humidity sensor that has many benefits that make it a great choice for this project.

- Low power consumption
- Comes calibrated from the factory lending to a great ease of use factor
- Very accurate readings
- Uses I2C 

There were a few other options for humidity sensors, but after looking around and weighing various options we decided on this humidity sensor due to its myriad of upsides.

<br>

<br>

## [Motor Controller](https://www.digikey.com/en/products/detail/infineon-technologies/IFX9201SGAUMA1/5415542)
<img src="https://mm.digikey.com/Volume0/opasdata/d220001/medias/images/376/P-PG-DSO-12.jpg" width="400" height="400">

We chose the Infineon Technologies IFX9201SGAUMA1 motor controller as it provides exactly the functionality needed for our design compared to other options. Additionally, we are familiar with the component, as we used it in our Advances Serial Communications assignment. Furthermore, we have example code that can be used to help us, as well as a working schematic.

- Built in H-Bridge allowing for easier control of our motor
- Has built in protection features such as over-current, over-temperature, and under-voltage lockout
- PWM interfaces
- It has a robust design that can handle harsh conditions
- The Advanced Serial Communications Assignment utilized this component, familiarizing us with it.



<br>

<br>

## [Battery](https://www.digikey.com/en/products/detail/panasonic-bsg/6LF22XWA-B/5067196)
<img src="https://mm.digikey.com/Volume0/opasdata/d220001/medias/images/1302/MFG_6LF22XWA.jpg" width="400" height="400">

For a battery we opted for a simple household 9V battery and we will be using a switching power regulator in order to get the voltage down to 3.3V to power all of our components. Many of our parts are very low power and our max current going through the system is also low, so a simple battery seemed to the best option.

<br>

<br>

## [Switching Power Supply](https://www.digikey.com/en/products/detail/onsemi/LM2575D2T-3.3R4G/5801702?utm_adgroup=&utm_term=&utm_content=&gad_source=1)
<img src="https://mm.digikey.com/Volume0/opasdata/d220001/medias/images/2468/D%C2%B2Pak%2CTO-263%3B%205%20Leads.jpg" width="400" height="400">

We are using a LM2575-3.3v this component is a simple switcher step-down voltage regulator. With this we will have a fixed output voltage of 3.3V. It can take voltages up to 40V with a 1A load.

<br>

<br>

## [Motor](https://www.digikey.com/en/products/detail/sparkfun-electronics/ROB-10846/5318748)
<img src="https://mm.digikey.com/Volume0/opasdata/d220001/medias/images/1164/MFG_ROB-10846.jpg" width="400" height="400">

We opted for the simple to use motor  ROB-10846 made by SparkFun Electronics. We wanted a robust motor that would also allow for easy control to help drive the movement of our solar panel. This motor is inexpensive but fits all of our design functions that we need.

<br>

<br>

## [Solar Panel](https://www.digikey.com/en/products/detail/anysolar-ltd/SM111K10L/9990439)
<img src="https://mm.digikey.com/Volume0/opasdata/d220001/medias/images/4431/MFG_SM111K10L.jpg" width="400" height="400">

Our onboard solar panel is configured in a diode ORing setup, enabling a split of the load between the 9V system and solar power. This design choice aligns with our commitment to the efficiency. The selected solar panel offers ample voltage for our circuit needs and the potential to support battery charging in future iterations. Most notably, the compactness of these solar cells is a key advantage, perfectly suiting the small form factor we are targeting. This configuration not only optimizes our energy management but also ensures our product remains portable.
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTYyOTI2MTE0NSwxNDEwNDA2NDI3LDkzMj
c4NTE5LDEwMDk4NzcxNzYsMjA0MDI5NzYyMl19
-->
