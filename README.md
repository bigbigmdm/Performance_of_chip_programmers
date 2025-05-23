# Performance_of_chip_programmers

## SPI operations time:

Tesitng computer: Intel(R) Core(TM)2 Duo CPU     E8400  @ 3.00GHz 5GB RAM

Testing chip: Winbond 25Q32 (4M)

| Programmer |       Software          |  Platform  | Reading | Erasing |  Writing | Veryfying |
| :---       |       :---              |     :---   |   :---: |   :---: |   :---:  |   :---:   |
| CH341A     | IMSProg v1.6.1          | Linux/GUI  |  33.9s  |  12.7s  | 328.5s   |   33.9s   |
| CH341A     | IMSProg table swap      | Linux/GUI  |  33.9s  |  11.4s  | 327.8s   |   33.9s   |
| CH341A     | SNANDer v.1.7.8         | Linux/CMD  |  33.0s  |   8.0s  | 327.0s   |   33.0s   |
| CH341A     | ch341prog               | Linux/CMD  | 135.3s  |   9.3s  | 359.5s   |  135.3s   |
| CH341A     | CH341a SPI programmer   | Linux/GUI  | 163.9s  |   9.5s  | 359.7s   |  163.8s   |
| CH341A     | flashrom v1.2           | Linux/CMD  |  34.6s  |  83.2s  | 132.7s   |   34.5s   |
| CH341A     | Ch341 Programmer 1.34   | Windows/GUI|  36.4s  |   9.0s  | 231.4s   |   36.4s   |
| CH341A     | NeoProgrammer 2.2.0.10  | Windows/GUI|  36.7s  |   9.1s  | 220.8s   |   36.7s   | 
| CH341A     | SiberiaProg 1.44        | Windows/GUI|  38.4s  |   9.5s  | 175.3s   |   38.4s   | 
| CH347T     | ch347-nor-prog          | Linux/CMD  |   1.1s  |   0.1s  |  28.9s   |    1.1s   |
| CH347T     | CH347_GUI_SPI_NOR_Flash_| Linux/GUI  |   1.6s  |   9.9s  |  35.0s   |   13.1s   |
| CH347T     | СH347 HighSpeed pr.v1.40| Windows/GUI|   0.7s  |  10.0s  |   8.1s   |    0.7s   |
| EZP2019+   | EZP2019+ Ver. 2.0       | Windows/GUI|  33.0s  |  10.4s  |  38.7s   |   33.0s   |

## Programmmer software features

| Programmer | Software                |  Platform  | SPI NOR| SPI NAND| I2C | MW | Edit SR | SFDP view | Secu-rity area view |.bin|.hex|.cap|
| :---       |       :---              |     :---   |:---:|:---:|:---:|:---:| :---:  |   :---:   |   :---:   |:---:|:---:|:---:|
| CH341A     | [IMSProg v1.6.1](https://github.com/bigbigmdm/IMSProg)         | Linux/GUI  | ✔   | -  | ✔   | ✔   |  ✔     |     ✔    |  ✔  | ✔ | ✔ | ✔ |
| CH341A     | [SNANDer v.1.7.8](https://github.com/McMCCRU/SNANDer)         | Linux/CMD  | ✔   | ✔   |+/-  |+/-  |  -     |     -     |  -  | ✔ | - | - |
| CH341A     | [ch341prog](https://github.com/setarcos/ch341prog)               | Linux/CMD  | ✔   | -  | -   | -   |  -     |     -     |  -  | ✔ | - | - |
| CH341A     | [CH341a SPI programmer](https://github.com/bigbigmdm/CH341a_spi_programmer)   | Linux/GUI  | ✔   | -  | -   | -   |  -     |     -     |  -  | ✔ | - | - |
| CH341A     | [flashrom v1.2](https://flashrom.org/)           | Linux/CMD  | ✔   | -   | -   |  -     |     -     |  -  | ✔ | - | - |
| CH341A     | [Ch341 Programmer 1.34](https://github.com/YTEC-info/CH341A-Softwares/blob/main/Programas/Windows/CH341Programmer/CH341Programmer%20V1.38/Ch341Programmer.exe?ysclid=ls2wxkusch126636141)   | Windows/GUI| ✔   | -   | ✔   |  -     |     -     |  -  | ✔ | ✔ |
| CH341A     | [NeoProgrammer 2.2.0.10](https://www.dwdvb.com/neoprogrammer-new-update-v2-2-0-10/)  | Windows/GUI| ✔   |  ✔ |   ✔  | ✔   |  ✔      |     -     |  -  | ✔ | ✔ | ✔ | ✔ |
| CH341A     | [SiberiaProg 1.44](https://ch341a.com/download/ch341a-siberiaprog-version-1-44)        | Windows/GUI| ✔   | -  |  ✔  | ✔   |  ✔     |     -     |  ✔  | ✔ | ✔ |
| CH347T     | [ch347-nor-prog](https://github.com/981213/ch347-nor-prog)          | Linux/CMD  | ✔   | -   | -   |  -     |     -     |  -  | ✔ | - | - |
| CH347T     | [СH347 HighSpeed pr.v1.40](http://www.yaojiedianzi.com/index.php?m=Product&a=show&id=19)| Windows/GUI| ✔   | -   | ✔   | ✔   |  -     |     -     |  -  | ✔ | ✔ |
| CH347T     | [CH347_GUI_SPI_NOR_Flash](https://github.com/bigbigmdm/CH347_GUI_SPI_NOR_Flash_programmer)| Linux/GUI| ✔   | -   | -   | -   |  -     |     -     |  -  | ✔ | - | - |
| EZP2019+   | [EZP2019+ Ver. 2.0](https://github.com/acontini/EZP2019)       | Windows/GUI| ✔   | -    | ✔  | ✔   |  -     |     -     |  -  | ✔ | ✔ | ✔ |

`✔` - yes.

`-`  - no.

`+/-` - is working, but errors have been detected.


**SPI NOR** - SPI NOR FLASH chips x25xxx series.

**I2C** - I2C chips 24xxx series.

**MW** - MicroWire chips 93xxx series.

**Edit SR** - View and edit SPI NOR FLASH status registers function.

**SFDP view** - view Serial Flash Discoverable Parameter register.

**Security area view** - Read/write SPI NOR FLASH OTP security registers.

**.bin** - .bin files format support.

**.hex** - Intel .hex files format support.

**.cap** - Asus .cap files format support.
