# Infrared_lantern
Powered By 18650 battery and two 350mA infrared LEDs. 

# Power supply:

option 1:
UFP（Upstream Facing Port), with 5.1K pulldown on CC1 and CC2, the ordinary power daptor for mobile phone can be used as input for the board;
AMS1117 is reserved to convert 5V to 3.3.

![image](https://github.com/user-attachments/assets/d04d7dc3-3858-46d8-8836-51f9448f3f26)
![image](https://github.com/user-attachments/assets/afec4184-2db7-4a56-83f5-f0555c0b664b)




option 2:
18650 Li battery is also supported as power source in the case. Note a Linear charge circuit(TP4056) is also available in this design, the battery can be charged from USB-C port direct;
Only one of TP4056 and AMS117 can be placed in specified design. However there are both available in the SCH/PWB.

![image](https://github.com/user-attachments/assets/bacdfb9d-7183-4066-92c1-9ca3313fe1e5)


Option 3:
reserved the vertical 2.54pitch power connector on the 3.3V net.


# MCU:
HK32F030MF4P6(TSSOP20 package, pin2pin compactable to STM8S003F3P6) is used as a Low cost(0.2~0.5 Dollar) "high" preformance MCU.
HK32F030M adopts the ARM® Cortex®-M0 core operating at a maximum frequency of 32 MHz.
USART/PWM/ADC/TIMER are all supported/

![image](https://github.com/user-attachments/assets/41e2d73c-29b5-4da5-9b9e-6f2bb7379fbe)


# Device:
Reset/Test Button; Two LED for debug propose; SWIO/SWCLK debug/progrom interface;  
![image](https://github.com/user-attachments/assets/0c95f87c-1726-4951-9e91-c025ef674937)

# LED driver and PIR sensor
MEL7135 is used as current source(350mA pre chip). SMT3030 infrared LED is used. SW1 is used of testing, in case the MCU is not used.
PIR sensor can be used as IRQ to MCU and futher opertion(enable the infrared LED) can be added if needed.
![image](https://github.com/user-attachments/assets/fb4450b8-45f0-48cb-92f2-2b0e63ed1383)

# M2 screw
the holes are added in each corner of the board.



#PCB

Top View

<img width="920" alt="image" src="https://github.com/user-attachments/assets/3d72d61b-30ee-44fb-a53a-e18510940468" />

Bottom View

<img width="870" alt="image" src="https://github.com/user-attachments/assets/90e3e9a0-e3f6-44fb-b028-1a8a29e22b9c" />



BOM:
![image](https://github.com/user-attachments/assets/f07806ee-6180-4ed9-aa98-42f62911ccf3)


