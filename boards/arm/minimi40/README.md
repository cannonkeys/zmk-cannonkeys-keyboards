# Minimi40 Wireless

This is the firmware for the CannonKeys developed Minimi40 Staggered Wireless PCB.

*Please make sure your PCB is the CannonKeys version before using this firmware*

## Charging Indicator

This PCB has a top-side charging indicator that can be toggled on and off. By default, it will turn on when the battery is charging.

If you'd like to turn it off, you can use the **Control Layer**. By default, the **Z** Key will turn the charging indicator on and **Left Control** will turn it off.

## Soft off functionality

This board supports ZMK Soft Off.

Soft off allows you to put the keyboard in an ultra low power state until you hit a specific key combination to wake it back up. The keyboard acts as if it is off - it does not advertise via BT nor work as a keyboard in bluetooth. It also preserves battery power.

This feature is especially useful on this PCB, as the battery switch is not accessible without removing a keycap.

By default the **BACKSPACE key** on the **Control Layer** triggers soft off mode. This can be remapped in ZMK Studio.

To turn the keyboard back on after soft off, you MUST press the following keys together:
- The topmost key in the first column of the keyboard. On the default keymap, this is **ESC**
- The 4th key down in the first column of the keyboard. On the default keymap, this is **LEFT CONTROL**

 This combination is defined by hardware and cannot be changed.

You can also exit soft off in a couple other ways. You can turn the battery off and on again using the switch, or hit the reset button on the bottom of the PCB to exit soft off.