# Bullet Train Wireless

This is the firmware for the CannonKeys Bullet Train Wireless PCB.

## Indicators

This PCB uses an RGB indicator in the top-left corner of the PCB to indicate a few things.

Upon boot, it will flash red, yellow, or green to indicate battery state. Red is 20%, Yellow is 0-80%, and Green is >80%

Upon boot or swapping Bluetooth profiles, it'll show BT connection status by flashing red, yellow, or blue. Red is not connected, yellow is not connected, but advertising, and blue is connected. Sometimes, if connecting to your PC is slow, the light will flash red to indicate no connection, shortly followed by blue. The speed of BT connection depends on your particular setup.

## ZMK Studio Unlock

By default, the **ENTER key** on the **Functional Layer** will unlock ZMK.

## Soft off functionality

This board supports ZMK Soft Off.

Soft off allows you to put the keyboard in an ultra low power state until you hit a specific key combination to wake it back up. The keyboard acts as if it is off - it does not advertise via BT nor work as a keyboard in bluetooth. It also preserves battery power.

This feature is especially useful on this PCB, as the battery switch is not accessible without removing a keycap.

By default the **BACKSPACE key** on the **Function Layer** triggers soft off mode. This can be remapped in ZMK Studio.

To turn the keyboard back on after soft off, you MUST press the following keys together:
- The left most key in the second row of the keyboard. On the default keymap, this is **ESC**
- The left most in the fourth row of the keyboard. On the default keymap, this is **LEFT SHIFT**

 This combination is defined by hardware and cannot be changed.

You can also exit soft off in a couple other ways. You can turn the battery off and on again using the switch, or hit the reset button on the bottom of the PCB to exit soft off.