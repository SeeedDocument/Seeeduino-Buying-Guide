---
title: Seeeduino Buying Guide
category: Tutorial
oldwikiname:  AT Command Tester
prodimagename:
surveyurl:
---

---
## Why we are here

Well，we have lots of Seeeduino Boards to achieve all kinds of functions.But you may find that it is difficult to make a choice among them all.So we make the list below and wish that it may help you.

## What's the difference

| products_name                                               | sku       |     Where to buy     | Micro Controller | Input Voltage | I/O Output Voltage | Clock Speed | Digital I/0 | Analoge Inputs | PWM | UART | Grove interface | FlashSpace | Boot loader       |
|-------------------------------------------------------------|-----------|----------|------------------|---------------|--------------------|------------|------------|--------------|-----|------|-----------------|------------|------------------|
| Seeeduino Mega                                              | 102010007 | [Purchase](https://www.seeedstudio.com/Seeeduino-Mega-p-717.html) | Atmega2560       | 7-12V         | 5V/3.3V            | 16MHZ      | 70         | 16           | 14  | 4    | 0               | 256K       | STK500v2         |
| Seeeduino Lotus - ATMega328 Board with Grove Interface      | 102020001 | [Purchase](https://www.seeedstudio.com/Seeeduino-Lotus-ATMega328-Board-with-Grove-Interface-p-1942.html) | Atmega328        | 7-12V         | 5V                 | 16MHZ      | 14         | 7            | 6   | 2    | 12              | 32K        | Optiboot         |
| Seeeduino V4.2                                              | 102010026 | [Purchase](https://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html) | Atmega328        | 7-12V         | 5V/3.3V            | 16MHZ      | 14         | 6            | 6   | 2    | 3               | 32K        | Optiboot         |
| Seeeduino Ethernet                                          | 102010000 | [Purchase](https://www.seeedstudio.com/Seeeduino-Ethernet-p-1231.html) | Atmega328P       | 7-12V         | 5V                 | 16MHZ      | 14         | 8            | 4   | 1    | 2               | 32K        | Arduino Ethernet |
| Seeeduino Stalker V3.1                                      | 102010070 | [Purchase](https://www.seeedstudio.com/Seeeduino-Stalker-V3.1-p-2686.html) | Atmega328P       | 3.7V          | 3.3V               | 8MHZ       | 14         | 6            | 0   | 1    | 2               | 32K        | Arduino Fio      |
| Seeeduino GPRS                                              | 102010016 | [Purchase](https://www.seeedstudio.com/Seeeduino-GPRS-p-1909.html) | Atmega32U4       | 9-12V         | 5V/3.3V            | 16MHZ      | 20         | 12           | 7   | 1    | 0               | 32K        | Caterina         |
| Seeeduino Lite                                              | 102010008 | [Purchase](https://www.seeedstudio.com/Seeeduino-Lite-p-1487.html) | Atmega32U4       | 7-12V         | 5V/3.3V            | 16MHZ      | 20         | 12           | 7   | 1    | 2               | 32K        | Caterina         |
| Seeeduino Cloud - Arduino Yun compatible openWRT controller | 102010021 | [![](https://github.com/SeeedDocument/Seeeduino-Buying-Guide/raw/master/img/Seeeduino%20Cloud.jpg)](https://www.seeedstudio.com/Seeeduino-Cloud-Arduino-Yun-compatible-openWRT-controller-p-2123.html) | Atmega32U4       | 7-12V         | 5V                 | 16MHZ      | 20         | 12           | 7   | 2    | 2               | 32K        | Caterina         |
| Seeeduino LoRaWAN                                           | 102010128 | [Purchase](https://www.seeedstudio.com/Seeeduino-LoRaWAN-p-2780.html) | ATSAMD21G18      | 3.7V          | 3.3V               | 48MHZ      | 14         | 6            | 18  | 2    | 4               | 256K       | Arduino Zero     |
| Seeeduino LoRaWAN W/GPS                                     | 102010129 | [Purchase](https://www.seeedstudio.com/Seeeduino-LoRaWAN-W-GPS-p-2781.html) | ATSAMD21G18      | 3.7V          | 3.3V               | 48MHZ      | 14         | 6            | 18  | 2    | 4               | 256K       | Arduino Zero     |

## In case you don't know
Microcontroller: The microcontroller is the heart (or, more appropriately, the brain) of the Arduino board. The Arduino development board is based on AVR microcontrollers of different types, each of which have different functions and features.

Input Voltage: This is the suggested input voltage range for the board. The board may be rated for a slightly higher maximum voltage but this is the safe operating range. A handy thing to keep in mind is that many of the Li-Po batteries that we carry are 3.7V meaning that any board with an input voltage including 3.7V can be powered directly from one of our Li-Po battery packs.

I/O Output Voltage: This is the voltage that the I/O pins can offer.

Clock Speed: This is the operating frequency of the microcontroller and is related to the speed at which it can execute commands. Although there are rare exceptions, most ATMega microcontrollers running at 3V will be clocked at 8MHz whereas most running at 5V will be clocked at 16MHz. The clock speed of the Arduino can be divided down for power savings with a few tricks if you know what you’re doing.

Digital I/O: This is the number of digital input/output pins that are broken out on the Arduino board. Each of these can be configured as either an input or an output, some are capable of PWM and some double as serial communication pins.

Analog Inputs: This is the number of analog input pins that are available on the Arduino board. Analog pins are labeled "A" followed by their number, they allow you to read analog values using the analog-to-digital converter (ADC) in the ATMega chip. Analog inputs can also be configured as more digital I/O if you need it!

PWM: This is the number of digital I/O pins that are capable of producing a PWM signal. A PWM signal is like an analog output, it allows your Arduino to “fake” an analog voltage between zero and the system voltage.

UART: This is the number of separate serial communication lines your Arduino board can support. On most Arduino boards, digital I/O pins 0&1 double as your serial send and receive pins and are shared with the serial programming port. Some Arduino boards have multiple UARTs and can support multiple serial ports at once. All Arduino boards have at least one UART for programming, but some aren't broken out to pins that are accessible.

Grove interface: Tells you how many Grove interface this board contains.

Flash Space: This is the amount of program memory that the chip has available for your to store your sketch. Not all of this memory is available as a very small portion is taken up by the bootloader (usually between 0.5 and 2KB).

Bootloader: If the microcontroller is the brain of the Arduino board, then the bootloader is its personality. Without the bootloader, it just wouldn’t be an Arduino. The bootloader lives on the ATMega chip and allows you to load programs through the serial port instead of having to use a hardware programmer. Because different Arduino board use different microcontrollers and programming interfaces, there are different bootloader programs on each. The source code for the bootloaders can be found in your Arduino distribution. All Arduino bootloaders will allow you to load code from the Arduino IDE.


## Want more

If you are still confused and need more information, just email us~~ tickets@seeed.uservoice.com
