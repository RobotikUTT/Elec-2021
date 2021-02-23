-----Components-----

PCA9685:
  - !OE pin: used to enable/disable all LED output at the same time.
    • When low applied to !OE, all outputs enabled (values follow datasheet p.16)
    • When high applied, all outputs follow the value defined by OUTNE[1:0] (p.27)

  - SDA/SCL pins: I2C communication.
    • I2C ADDRESS : 1 + A5 + A4 + A3 + A2 + A1 + A0 + R/W
    • Don't forget the pullups.

  - EXTCLK : External clock, used to synchronize multiple PCA9685 startups.

  - Pins are 5V tolerant
