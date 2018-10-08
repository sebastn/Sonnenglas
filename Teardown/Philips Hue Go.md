# Philips Hue Go Teardown

The file includes the various steps involved in the teardown of **Philips Hue Go** smart lamp and the information about the  different components used in it.

## Teardown Procedure
### 1. 
![The base layer is pried open](/Teardown/images/Philips Hue Go/1.jpg)

The base layer (Reflector/Light diffuser?) is pried open and the the 4 LEDs are exposed. It's expected that the LEDs are RGBW and are the primary components of the Philip Hue Go.

### 2.
![](/Teardown/images/Philips Hue Go/2.jpg)

The removal of the plastic casing exposes the PCB board which houses the LEDs and also the remaining components involved in the circuit.
### 3.
![](/Teardown/images/Philips Hue Go/3.jpg)

Beneath the PCB Board there's a metal weight which serves the purpose of balanceing the light in an inclined position and also in adding up to the weight of the lamp which otherwise would be too light.

### 4.
![](/Teardown/images/Philips Hue Go/4.jpg)

Upon removal of the metal weight, we can see the battery holder and 2 X **3.7 V** AA Li-ion Batteries (14500 size battery each ***680mAh***). The lamp lasts for upto ***3 hours*** on battery.

### 5.
![](/Teardown/images/Philips Hue Go/5.jpg)

The image shows the battery holder and the connection which goes to the PCB. Beneath this board is a push button on the Hue go which controls the different modes of the lamp.


## PCB and Components
![enter image description here](/Teardown/images/Philips Hue Go/6.jpg)

The PCB does not seem to be too complicated but it is well designed and well laid out (as compared to the Roome Device which was also tore down on 18th September 2018).

The SoC used here is the Atmel ***ATmega2564RFR2*** (datasheet - https://www.microchip.com/wwwproducts/en/atmega2564rfr2#additional-features).
*Primary Features*:
- An IEEE 802.15.4 compliant single chip which combines an industry-leading AVR microcontroller and best-in-class 2.4GHz RF transceiver.
- Supports 4-wire SPI, TWI, ISP, JTAG, UART, USART
- Very low power consumption:
-- 9.6mA in RX mode
-- 16.4mA in TX mode
-- 0.6μA in sleep mode

It also has a MX25L4006E CMOS Serial Flash Memory which might be holding the different modes/presets of the Hue Go Lamp.

The different possible circuits in the Main PCB are:

- A Battery Charging Circuit whose connection goes to the battery holder arrangement mentioned above
- An LED Driver circuit consisting of multiple MOSFETs. The MOSFETs might be Pulse-Width Modulated inorder to adjust the brightness of the LEDs.

# Comparison with Roome

The **Philips Hue Go** Circuit is not so complicated, neither are the components expensive. The market price of the product is way more than the actual production cost. The main highlight of the product is that it very ***elegent*** and it does its job perfectly. The product has an amazing finish and the light diffuser makes the light output really pleasant.

On the other hand, the **Roome** product, which is offered by a Chinese company packs a lot of features into one product which costs almost the same price as the Philips Hue Go. It has
-   Motion-sensor technology：IR Sensor
-   Brightness adjustment: Using special ambient light sensing technology roome will automatically choose the perfect level of brightness (LDR used inside)
-   Simple gesture-control operation: which does not function properly. Once we move the hand above its maximum operating range, it turns off (which is not the expected behaviour). When the hand is closest to the product it is at its lowest brightness and as we move up the brightness increases. But the product was operating erratically.
-   Can work as a Power Bank - 2 X 5V 1 A USB ports
-   App control - It was really difficult to setup the product. It had issues pairing with the android device as well as connecting to a WiFi network having a password. (We made it work by connecting to an open WiFi hotspot).
- Control by Tapping - uses vibration sensor inside
- Bluetooth Music Play - uses a direct bluetooth music receiver IC and the output is connected to a not so great speaker.

The Roome product does not feel premium and the plastic casing also looks cheap. The light output is not impressive.

# Takeaway
From the point of view of a customer, I would prefer to use a product which has limited functionalities but which works in a simple manner and in a perfect fashion. Philips Hue Go, although it does not have a lot of features, does its job perfectly and its really impressive.

Suggestions for Sirius:
- Keep device pairing as simple as possible.
- Focus on offering limited functions which function perfectly rather than including a lot of features.
