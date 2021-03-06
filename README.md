# Rocket Panda Mk. I
# [Full write-up is on my website!](https://iamericmin.github.io/rocketpanda1.html)

## nRF52832 dev kit designed for experiments with BLE

Project status: very early in development. THIS IS A PROTOTYPE AND IS CURRENTLY VERY MESSY!

# What is this?
The Rocket Panda is an nRF52832 dev kit that I will use to prototype my future projects. I already have the nRF52832-DK, but I believe the best way to learn a chip is to make a breakout board for it. This is also my first ever project with a built in USB-serial converter. The Rocket Panda gets the funky name from its black and white PCB.

# SPEC SHEET:
- PROCESSOR: nRF52832 Soc. 64MHz ARM cortex M4 with 64k RAM and 512k flash
- BOOTLOADER: Adafruit custom nRF52 DFU bootloader
- CONNECTORS: Triple 2x10 2.54mm pin headers, Cortex debug header, JST-PH Serial connector, USB serial connector
- I/O: Reset button, user button, power LED, RX/TX LEDs, and two auxilliary LEDs.
- POWER: CR2032 coin cell or USB mini-B jack
- DIMENSIONS: Credit card size(85.6mm x 54mm)

# Repo structure
The rocketpanda_fw folder contains everything related to the Rocket Panda's firmware. This includes a Platform IO project folder, Adafruit's custom DFU bootloader, and Nordic's J-Link recovery firmware for the nRF52DK.
The rocketpanda_hw folder contains everything hardware related, such as eagle files, schematics, and BOM. It also includes the hardware files for Adafruit's nRF52832 feather board since I used it as a close reference when designing the Rocket Panda.
