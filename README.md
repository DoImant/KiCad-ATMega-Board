# ATMega Board

The usual Arduino boards like the Arduino Uno , Nano, Mini etc. are only conditionally suitable for battery operation.

The current requirement of the built-in LEDs, the USB-UART interface and the quite high quiescent current of the LDO regulator is too high for a longer operation on a battery, even if the microcontroller is in sleep mode.

On the ATMega board only the most necessary components are installed, which are necessary for the operation of a microcontroller. This makes it possible to operate the controller with batteries for a longer time. The screw terminals allow stable and trouble-free connections with external components.

With the help of a jumper the power indicator LED (consumes about 3mA) can be switched on or off as needed. 

## Limitations compared to the usual Arduino boards  

* Programming must be done via the ISP adapter.
* For serial communication an external FTDI adapter is required.
* The analog ports A6 and A7 (e.g. compared to an Arduino Nano) are not available.
* No 3.3V output. But you can use the whole board instead of a 5V LDO with a 3.3V LDO (MCP-1703-3302MB
 or HT7833-1).


## Other technical data

* Usable microcontrollers: ATTiny88, ATmega48A/PA, 88A/PA, 168A/PA, 328/P
* The crystal is exchangeable (depending on the inserted microcontroller max. 20Mhz)
* Supply voltage via JST XH connector or VIN-Pin min. 6V, max. 15V
* Max. 200mA current load (the LDO has a limit of 250mA, the AVR controllers 200mA.)
* Power consumption with an ATMega328P in sleep mode *"SLEEP_MODE_PWR_DOWN"* and disabled ADC < 10µA

## Circuit diagram as PDF file

[Sheet](https://github.com/DoImant/Stuff/blob/main/ATMega-Board/ATMega-Board.pdf)

## The PCB

![PCB](https://github.com/DoImant/Stuff/blob/main/ATMega-Board/ATMega-Board-PCB.png?raw=true)

![3D-Image](https://github.com/DoImant/Stuff/blob/main/ATMega-Board/ATMega-Board-PCB-3D.png?raw=true)

![Picture](https://github.com/DoImant/Stuff/blob/main/ATMega-Board/ATMegaboard-1024.jpg?raw=true)

