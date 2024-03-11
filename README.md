# N76e003 UFO Target board for the Chipwhisper UFO board

Tested and working, gerbers are in `jlcpcb/`

# Note
ChipWhisperer normally has gpio1 set as serial_rx and gpio1 set as serial_tx; this is reversed on the current board. This will be fixed in the next revision. When using the current board, just set:
```python
scope.io.tio1 = "serial_tx"
scope.io.tio2 = "serial_rx"
```
