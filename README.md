# Steelseries Rival 310 protocol specification

### Commands

Value | Command | Link
:---: | --- | :---:
`0x00-0x01` | Reset (same as unplugging and plugging the mouse) | [01](https://github.com/FFY00/rival310-re/blob/master/01.md)
`0x3 + 0x05` | Used for firmware updates (seriously, **don't use**) |
`0x07` | Old led effect command (works only partialy, don't use) |
`0x08` | Old led color command (works only partialy, don't use) |
`0x09` | Old save command **DON'T USE!! This will break the LEDs** |
`0x31` | Set button action |
`0x33` | Uknown, has something to do withy the buttons (at least the wheel) | [33](https://github.com/FFY00/rival310-re/blob/master/33.md)
`0x40` | Unkown. Seems to fix LEDs after `0x09` |
`0x53` | Changes DPI | [54](https://github.com/FFY00/rival310-re/blob/master/53.md)
`0x54` | Changes polling rate | [54](https://github.com/FFY00/rival310-re/blob/master/54.md)
`0x59` | Save | [59](https://github.com/FFY00/rival310-re/blob/master/59.md)
`0x5A` | Unknown, has something to do with the DPI | [5A](https://github.com/FFY00/rival310-re/blob/master/5A.md)
`0x5B` | Configure cycle (LEDs) | [5B](https://github.com/FFY00/rival310-re/blob/master/5B.md)
`0x60` | Resets cycle |
`0x87` | Uknown (Gets value*) |
`0x89` | Uknown (Gets value*) | [89](https://github.com/FFY00/rival310-re/blob/master/89.md)
`0x90` | Gets the firmware version | [90](https://github.com/FFY00/rival310-re/blob/master/90.md)
`0x91` | Uknown (Gets value*) |
`0x92` | Uknown (Gets value*) | [92](https://github.com/FFY00/rival310-re/blob/master/92.md)
`0x9A` | Uknown (Gets value*) |
`0xD4` | Uknown (Gets value*) |
`0xD6` | Uknown (Gets value*) |
`0xFC` | Uknown (Gets value*) |
`0xFD` | Uknown (Gets value*) |
`0xFE` | Uknown (Gets value*) | [FF](https://github.com/FFY00/rival310-re/blob/master/FE.md)
`0xFF` | Enable button report |

* - When the command is sent, the device returns a packet with data. May not always work.
