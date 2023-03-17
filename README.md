# esp32-guitar-pedal
This project is a way to make an all purpose guitar pedal using an ESP32.

# Goals 
## Pedal Types
1. Tuner
2. Distortion
3. Noise Gate
4. Delay

# Software
## Board Initilization
### GPIO
### DAC
### ADC
### INT
### RF
Disable WiFi/BLE
## Tuner
If SELSW1 depressed > 3 sec -> tune()
## Distortion
if (input_signal > Samples/2 + distortion_value) input_signal= Samples/2 + distortion_value;
if (input_signal < Samples/2 - distortion_value) input_signal= Samples/2 - distortion_value;
## Noise Gate
If Vin < x, Vout = 0. Linear
## Delay
Timeshifting 
# Hardware
## Parts List
1. ESP32
2. [Monochrome 1.3" 128x64 OLED graphic display] (https://www.adafruit.com/product/938)
3. [¼ Enclosed Mono Jack, Lugs] (https://guitarpedalparts.com/collections/1-4-jacks/products/1-4-enclosed-mono-jack-lugs)
4. Power [DC Barrell Jack 2.1mm center pin](https://guitarpedalparts.com/collections/power/products/dc-jack-internal-nut)
5. Selecion knobs [PEC11R Series - 12 mm Incremental Encoder](https://www.bourns.com/docs/product-datasheets/pec11r.pdf)
6. Foot Switches [SPST Momentary Soft Touch Foot Switch, Normally Open](https://guitarpedalparts.com/collections/switches-momentary/products/spst-momentary-soft-touch-foot-switch)  
7. Enclosure [1590DD Aluminum Die-Cast Enclosure](https://guitarpedalparts.com/collections/switches-momentary/products/spst-momentary-soft-touch-foot-switch)
