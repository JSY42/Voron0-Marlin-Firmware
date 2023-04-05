# Voron0-Marlin-Firmware
Marlin Firmware that I use for my voron0

Used the latest bugfix 2.1.x
downloaded from https://github.com/MarlinFirmware/Marlin
( 04/04/2023 current version 02010300 )

Based on MKS Eagle Motherboard
https://www.aliexpress.com/item/1005003352842756.html

Uses MKS mini 12864 V3 lcd.

Has no Mesh leveling nor abl enabled ( cuz it's a small bed )


How to use : 

1. Download the lastest marlin version (check if it is the same!)
2. Replace Configuration.h and Configuration_adv.h in "Marlin" folder with the downloaded ones on this git
3. Also put in Bootscreen.h file into "Marlin" folder ( the same folder with configs ) If u want to use the custom bootscreen.
4. Replace Marlin/src/pins/stm32f4/pins_MKS_ROBIN_NANO_V3_common.h with the downloaded one on this git. (read below)
5. Compile - by either platformio or abm / OR you could just use the already compiled .bin file on this git.
6. Put the .bin file into sd card and insert it to the motherboard.

p.s. the firm's mostly based on my use...
I use 3 controlled fans - fan0 for the cooling fan, fan1 for the hotend fan, and fan2 uses the e1 heater pin (PB1)- I connected my Nevermore filter fan to it.
The driver cooling fans are connected to 24v output.
So if u dont need such features, skip step 4.
