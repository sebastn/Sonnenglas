# Hardware Research
The selection of the hardware components is dependend on the feature list and the desired technical specifications. The current requirements are

- Bluetooth Low Energy support
- 802.15.4 Zigbee support
- BLE mesh ability
- Multiple input power management: solar, usb, induction
- Battery operated
- Digital RGB LED control
- Constant current supply for LEDs
- Touch botton control
- (Touch) gesture control

## Power consumption estimation
The overall battery life is mainly dependend on the LED brightness. 
The current draw of electronic parts is mainly consumed by the radio (BLE and Zigbee).

The following estimations only takes the MCU without its peripherals into account. Current draw for active radio receiving (RX) and CPU standy are added. This will be the most common operation mode and will roughly represent the actual usage. The estimated runtime assume a battery capacity of 2500mAh at 3.7V (9.25Wh).

### Nordic NRF52480
The datasheet stats a current draw of 4.6mA RX at 1Mbps. 
The system current draw is 1.5μA at System ON mode.

Rounding up to 5mA (at 3V) of total current draw at active receiving mode, the power consumption is at 0.015W. The chip-only runtime will be 616h (25.5 days). 

### Silicon Labs CC2652R
The radio current draw 6.83 mA at active RX mode. 
The system current draw at stand-by is 0.92 µA.

The total system current draw will be at around 7mA, making the power consumption 0.021W. The chip-only runtime will be 440.5h (18.3 days).
