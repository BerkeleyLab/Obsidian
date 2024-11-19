# Marble Tiny

## Description

Marble Tiny is a (proposed) FPGA carrier board, designed to interface with ADC and DAC devices,
either standalone or as an I/O expansion board for [Marble](https://github.com/BerkeleyLab/Marble).

## Major Parts

- Xilinx XC7A50T-1CSG325C FPGA

## Credits

## License

---

## Project status

### Included features

- [ ] Arduino shield compatible, like the Digilent Arty
- [ ] SPI flash boot
- [ ] DDR3 memory chip
- [ ] FTDI USB interface
- [ ] 2 direct LEDs
- [ ] 1 GigE port (PoE?)
- [ ] 6 Pmod ports (3.3V)
- [ ] MS5351M or SI5351A or similar for GTP frequency reference
- [ ] USB-C (single USB cable)
- [ ] 4 x SFP
- [ ] i2c or 1-wire chip for serial number / rom 
- [ ] White Rabbit

### High speed links

The 7A50T-1CSG325C has 4 x GTP lanes, capable of 3.75 Gbaud.
The primary use-case involves attaching one of those to a Marble over fiber.

### Wishlist

- [ ] Standardized board size for good case options: Mini-ATX (150 x 150 mm)? Pico-ATX?

### Pins
- 48 pins for 6 PMODs
- 13 pins for RGMII (including reset pin)
- 6 pins for White Rabbit
- 2 pins for I2C
- 14 pins for Arduino digital IO
- 8 pins for Arduino 4 analog channels 
- 49 pins for DDR3
- 2 pins USB - UART
- 2 Ethernet PHY MDIO
- 4 WR SPI DAC
- 1 or more clock input (some clocks can come in on GTPREFCLK).
