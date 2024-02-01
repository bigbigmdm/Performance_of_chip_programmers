# Performance_of_chip_programmers

## SPI operations time:

Tesitng computer: Intel(R) Core(TM)2 Duo CPU     E8400  @ 3.00GHz 5GB RAM

Testing chip: Winbond 25Q32 (4M)

| Programmer |       Software        |  Platform  | Reading | Erasing |  Writing | Veryfying |
| :---       |       :---            |     :---   |   :---: |   :---: |   :---:  |   :---:   |
| Ch341a     | IMSProg v1.1.10       | Linux/GUI  |  33.9s  |  11.4s  |  328.5s  |   33.9s   |
| Ch341a     | IMSProg table swap    | Linux/GUI  |  33.9s  |  11.4s  | 327.8s   |   33.9s   |
| Ch341a     | SNANDer v.1.7.8       | Linux/CMD  |  33.0s  |   8.0s  | 327.0s   |   33.0s   |
| Ch341a     | ch341prog             | Linux/CMD  | 135.3s  |   9.3s  | 359.5s   |  135.3s   |
| Ch341a     | CH341a SPI programmer | Linux/GUI  | 163.9s  |   9.5s  | 359.7s   |  163.8s   |
| Ch341a     | flashrom v1.2         | Linux/CMD  |  34.6s  |  83.2s  | 132.7s   |   34.5s   |
| Ch341a     | Ch341 Programmer 1.34 | Windows/GUI|  36.4s  |   9.0s  | 231.4s   |   36.4s   |
| Ch341a     | NeoProgrammer 2.2.0.10| Windows/GUI|  36.7s  |   9.1s  | 220.8s   |   36.7s   | 
| Ch341a     | SiberiaProg 1.44      | Windows/GUI|  38.4s  |   9.5s  | 175.3s   |   38.4s   | 
| Ch347a     | ch347-nor-prog        | Linux/CMD  |   1.1s  |   0.1s  |  28.9s   |    1.1s   |
| EZP2019+   | EZP2019+ Ver. 2.0     | Windows/GUI|  33.0s  |  10.4s  |  38.7s   |   33.0s   |

## Programmmer software features

| Programmer | Software               |  Platform  | SPI | I2C | MW | Edit SR | SFDP view |
| :---       |       :---             |     :---   |:---:|:---:|:---:| :---:  |   :---:   |
| Ch341a     | IMSProg v1.1.10        | Linux/GUI  | +   | +   | +   |  +     |     +     |
| Ch341a     | IMSProg table swap     | Linux/GUI  | +   | +   | +   |  +     |     +     |
| Ch341a     | SNANDer v.1.7.8        | Linux/CMD  | +   |+/-  |+/-  |  -     |     -     |
| Ch341a     | ch341prog              | Linux/CMD  | +   | -   | -   |  -     |     -     |
| Ch341a     | CH341a SPI programmer  | Linux/GUI  | +   | -   | -   |  -     |     -     |
| Ch341a     | flashrom v1.2          | Linux/CMD  | +   | -   | -   |  -     |     -     |
| Ch341a     | Ch341 Programmer 1.34  | Windows/GUI| +   | +   | -   |  -     |     -     |
| Ch341a     | NeoProgrammer 2.2.0.10 | Windows/GUI| +   | +   | +   |  -     |     -     |
| Ch341a     | SiberiaProg 1.44       | Windows/GUI| +   | +   | +   |  +     |     -     |
| Ch347a     | ch347-nor-prog         | Linux/CMD  | +   | -   | -   |  -     |     -     |
| EZP2019+   | EZP2019+ Ver. 2.0      | Windows/GUI| +   | +   | +   |  -     |     -     |


