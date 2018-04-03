# Steelseries Rival 310 protocol specification

### Commands

Value | Command | Link
:---: | --- | :---:
`0x00 + 0x01` | Reset (same as unplugging and plugging the mouse) | [01](https://github.com/FFY00/rival310-re/blob/master/01.md)
`0x03 + 0x05` | Used for firmware updates (seriously, **don't use**) |
`0x07` | Old led effect command (works only partialy, don't use) |
`0x08` | Old led color command (works only partialy, don't use) |
`0x09` | Old save command **DON'T USE!! This will break the LEDs** |
`0x31` | Set button action |
`0x33` | Uknown, has something to do with the buttons (at least the wheel) | [33](https://github.com/FFY00/rival310-re/blob/master/33.md)
`0x40` | Resets the LEDs. Seems to fix LEDs after `0x09` |
`0x53` | Changes DPI | [53](https://github.com/FFY00/rival310-re/blob/master/53.md)
`0x54` | Changes polling rate | [54](https://github.com/FFY00/rival310-re/blob/master/54.md)
`0x59` | Save | [59](https://github.com/FFY00/rival310-re/blob/master/59.md)
`0x5A` | Unknown, has something to do with the DPI | [5A](https://github.com/FFY00/rival310-re/blob/master/5A.md)
`0x5B` | Configure cycle (LEDs) | [5B](https://github.com/FFY00/rival310-re/blob/master/5B.md)
`0x60` | Resets cycle |
`0x87` | Read current color from LED 1 |
`0x89` | Uknown (Reads value*) | [89](https://github.com/FFY00/rival310-re/blob/master/89.md)
`0x90` | Reads the firmware version | [90](https://github.com/FFY00/rival310-re/blob/master/90.md)
`0x91` | Uknown (Reads value*) |
`0x92` | Reads mouse values (DPI and LEDs) | [92](https://github.com/FFY00/rival310-re/blob/master/92.md)
`0x9A` | Uknown (Reads value*) |
`0xD4` | Uknown (Reads value*) |
`0xD6` | Uknown (Reads value*) |
`0xFC` | Uknown (Reads value*) |
`0xFD` | Uknown (Reads value*) |
`0xFE` | Uknown (Reads value*) | [FE](https://github.com/FFY00/rival310-re/blob/master/FE.md)
`0xFF` | Enable button report |

`*` - When the command is sent, the device returns a packet with data. May not always work.

### Force firmware update (reset)
  * Unplug the mouse
  * Press all the buttons for 10s
  * Plug the device still pressing the buttons

Now the LEDs should start blinking and you will be forced to update the firmware. Please note this **is not** a factory reset, it will only force the firmware to be updated.
