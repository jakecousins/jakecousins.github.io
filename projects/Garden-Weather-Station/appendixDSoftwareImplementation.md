## Humidity Sensor Code

#include "mcc_generated_files/pin_manager.h"

#include "mcc_generated_files/mcc.h"

#include "mcc_generated_files/hdc1000.h"

#include "mcc_generated_files/eusart2.h"

#include <stdio.h>

#include "mcc_generated_files/i2c2_master.h"

#include "mcc_generated_files/examples/i2c2_master_example.h"

#include <string.h>

void main(void) 
{
    // Initialize the device
    SYSTEM_Initialize();

    // Enable the heater if needed
    HDC1000_EnableHeater(true);

    // Initialize EUSART2
    EUSART2_Initialize();

    // Read temperature and humidity
    float temperature = HDC1000_GetTemp();
    uint8_t humidity = HDC1000_GetHumidity();
    
     // Set LED pin as output
    LED_SetDigitalOutput();
    
    LED_SetHigh();
    
    while (1) {
       
        if(HDC1000_GetHumidity() >= 50) 
        {
            LED_SetHigh();  // Turn on the LED
            //__delay_ms(50);
        } 
        else 
        {
            LED_SetLow();   // Turn off the LED
        }
    }

    // Print the temperature and humidity
    //printf("Temperature: %.2f degrees C, Humidity: %d%%\r\n", temperature, humidity);

    // Disable the heater if it was enabled
    HDC1000_EnableHeater(false);
}

## Motor Code

#include "mcc_generated_files/mcc.h"

uint8_t FWD = 0b11101111;  // Forward command
uint8_t BWD = 0b11101101;  // Backward command
uint8_t data;

int main(void)
{
    // Initialize the system, SPI, and EUSART
    SYSTEM_Initialize();
    SPI1_Open(SPI1_DEFAULT);
    EUSART2_Initialize();

    while (1)
    {
        // Set CSN low, send the forward command, and then set CSN high
        CSN_SetLow();
        data = SPI1_ExchangeByte(FWD);
        CSN_SetHigh();
        printf("Forward data: %x \r\n", data);
        //__delay_ms(1000);  // Forward for 1 second
        
        if(data = SPI1_ExchangeByte(FWD))
        {
            LED_SetHigh();
        }
        // Delay for 3 seconds before changing direction
        __delay_ms(3000);
           
       
        // Set CSN low, send the backward command, and then set CSN high
        CSN_SetLow();
        data = SPI1_ExchangeByte(BWD);
        CSN_SetHigh();
        
         
        
        printf("Backward data: %x \r\n", data);
        //__delay_ms(1000);  // Backward for 1 second
        
        LED_SetLow();
        // Delay for 3 seconds before changing direction again
        __delay_ms(3000);
    }
}
