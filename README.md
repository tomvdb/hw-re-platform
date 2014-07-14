Hardware Reverse Engineering Learning Platform
==============================================

Current Status:

2014/07/17: Boards received, concept works, pcb has some minor issues. Working on v2
2014/06/20: PCB's sent for manufacturing - Not Tested Yet

I enjoy trying to reverse engineer the famous crackme and reverseme executables in my spare time. After reading the xbox reverse engineering book by bunnie I went looking at the my options for learning and experimenting with hardware reverse engineering. Unfortunately the options are few and expensive.

The hardware reverse engineering platform is basically a shield for the new stm32 nucleo boards using the st-morpho connectors. It contains two arduino compatible microcontrollers and an eeprom. There are 8 data lines connected between the two microcontrollers and there is also i2c lines connecting the mcu's with an eeprom. The nucleo board handles loading the reverse engineering scenario on the shield (firmware on the avr's and data on the eeprom). Test pins are added on all the data lines for connection to RE tools. This allows anyone to easily create firmware that depicts a possible RE situation. For example the two mcu's can communicate with each other using a certain protocol.

