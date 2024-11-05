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

- [ ] At least one high-speed fiber; see below
- [ ] 1 GigE port
- [ ] 4 Pmod ports
- [ ] MS5351M or SI5351A or similar for GTP frequency reference
- [ ] FTDI USB interface
- [ ] Arduino shield compatible, like the Digilent Arty

### High speed links

The 7A50T-1CSG325C has 4 x GTP lanes, capable of 3.75 Gbaud.
The primary use-case involves attaching one of those to a Marble over fiber.
Possible hardware configurations that would meet that need,
and enable other interesting I/O:

- [ ] 1 x QSFP
- [ ] 4 x SFP
- [ ] 2 x SFP and 2 x SATA

#### SATA related features

The SATA connectors are intended to provide Marble Tiny peer-to-peer communication while the optical connector provides communication with Marble. Furthermore, the SATA standard allows to interface with commercial storage devices like SSD or HDD in order to memorize the sampled data. Possible use cases could be gathering of large dataset for machine learning, or any diagnostic purpose.

### Wishlist

- [ ] Standardized board size for good case options: Mini-ATX (150 x 150 mm)?
- [ ] Pmod directly connected to 3V3 FPGA pins (no bidirectional buffer chips)
- [ ] Pmod pin number printed on PCB
- [ ] DDR3 memory chip
- [ ] White Rabbit
- [ ] USB-C powered
- [ ] Serial number shared between FTDI and FPGA
