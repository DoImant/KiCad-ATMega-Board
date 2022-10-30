# ATMega Board

The usual Arduino boards like the Arduino Uno , Nano, Mini etc. are only conditionally suitable for battery operation.

The current requirement of the built-in LEDs, the USB-UART interface and the quite high quiescent current of the LDO regulator is too high for a longer operation on a battery, even if the microcontroller is in sleep mode.

On the ATMega board only the most necessary components are installed, which are necessary for the operation of a microcontroller. This makes it possible to operate the controller with batteries for a longer time. The screw terminals allow stable and trouble-free connections with external components.  

## Limitations compared to the usual Arduino boards  

* Programming must be done via the ISP adapter.
* For serial communication an external FTDI adapter is required.
* The analog ports A6 and A7 (e.g. compared to an Arduino Nano) are not available.

## Other technical data

* Usable microcontrollers: ATTiny88, ATmega48A/PA, 88A/PA, 168A/PA, 328/P
* The crystal is exchangeable (depending on the inserted microcontroller max. 20Mhz)
* Supply voltage via JST XH connector min. 6V, max. 15V
* Max. 200mA current load (the LDO has a limit of 250mA, the AVR controllers 200mA.)

## Circuit diagram as PDF file

[Sheet](https://github.com/DoImant/Stuff/blob/main/ATMega-Board/ATMega-Board.pdf)

## The PCB

![PCB](https://github.com/DoImant/Stuff/blob/main/ATMega-Board/ATMega-Board-PCB.png?raw=true)

![Picture](https://github.com/DoImant/Stuff/blob/main/ATMega-Board/ATMegaboard-1024.jpg?raw=true)
