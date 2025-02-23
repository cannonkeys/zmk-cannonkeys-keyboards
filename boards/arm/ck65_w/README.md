# CK 65 Wireless

This is the CannonKeys 65% Wireless PCB Firmware
It's compatible with Bakeneko65, Brutal v2 65, and Bakeneko65, among others.

```
west build -p -b ck65_w
```

## Soft off functionality

This board supports ZMK Soft Off.

Soft off allows you to put the keyboard in an ultra low power state until you hit a specific key combination to wake it back up. The keyboard acts as if it is off - it does not advertise via BT nor work as a keyboard in bluetooth. It also preserves battery power.

This feature is especially useful on this PCB, as the battery switch is not accessible without removing a keycap.

By default the **BACKSPACE key** on **Layer 2** triggers soft off mode. This can be remapped in ZMK Studio.

To turn the keyboard back on after soft off, you MUST press the following keys together:
- The topmost key in the last column of the keyboard. On the default keymap, this is **DEL**
- The 4th key down in the last column of the keyboard. On the default keymap, this is **MO(1)**

 This combination is defined by hardware and cannot be changed.

You can also exit soft off in a couple other ways. You can turn the battery off and on again using the switch, or hit the reset button on the bottom of the PCB to exit soft off.