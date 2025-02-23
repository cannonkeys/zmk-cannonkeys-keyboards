# CK60 Wireless

This PCB is currently used for the following boards:
- Vida
- Bakeneko GO (Purchased in 2025 or later)

## Soft off functionality

This board supports ZMK Soft Off.

Soft off allows you to put the keyboard in an ultra low power state until you hit a specific key combination to wake it back up. The keyboard acts as if it is off - it does not advertise via BT nor work as a keyboard in bluetooth. It also preserves battery power.

This feature is especially useful on this PCB, as the battery switch is not accessible without removing a keycap.

By default the **ENTER key** on **Layer 2** triggers soft off mode. This can be remapped in ZMK Studio.

To turn the keyboard back on after soft off, you MUST press the keys that are mapped to **Right Ctrl** and **Enter** in the default keymap. This is defined by hardware and cannot be changed.

You can also exit soft off in a couple other ways. You can turn the battery off and on again using the switch, or hit the reset button on the bottom of the PCB to exit soft off.