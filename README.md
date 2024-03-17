# N76e003 UFO Target board for the Chipwhisper UFO board

Tested and working, gerbers are in `jlcpcb/`

# Note
ChipWhisperer normally has gpio1 set as serial_rx and gpio1 set as serial_tx; v1.1 and earlier of this board had this reversed. v1.2 and later fixes this issue. When using these earilier boards, just set:
```python
scope.io.tio1 = "serial_tx"
scope.io.tio2 = "serial_rx"
```

The shunt resistor value is 22R, which is likely too high, given that the max current is 3.9mA operating at 16mhz. I have not had a chance to test additional shunt resistor values, but I would recommend using a lower value, such as 11R.