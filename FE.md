# Specification of the `FE` command
### Unknown command

**(0) Specification**

Byte (Index) | Explanation | Values
:---: | --- | ---
`0` | Command | `FE`
`1-End` | Unknown | `00`

**(1) Example reply**

Like `90`, the mouse can reply to this command. Here's the reply I was able to get.
```
36 32 34 33 33 33 30 34 30 34 33 38 31 37 30 34
31 37 37 00 00 00 00 00 00 00 00 00 00 00 00 00
00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00
00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00
```
