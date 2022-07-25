# Moisture_Click_for_Arduino
Library of Moisture_click Modules Using Texas Instruments' FDC2112

# Usage
Include header, Make instance, Init and acquire data.

```cpp
#include <Wire.h>
#include "Moisture_Click_for_Arduino.h"
FDC2112 capsense(MOISTURE_DEV_ADR_GND); // Use FDC2112_I2C_ADDR_1 

...
void setup() {
    ...
    Wire.begin(); /if ESP32, Wire.begin(23, 22)
    bool capOk = capsense.begin(); 
    ...
}
void loop(){
    ...
        moisture_get_data();
    ...
}
```

# Reference
This library was created by referring to the link below.
>* Official library of Moisture Click module : https://github.com/MikroElektronika/Moisture_click   
>* FDC2XXX library : https://github.com/zharijs/FDC2214
