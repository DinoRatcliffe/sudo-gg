# sudo-gg
Gives appropriate response to the use of sudo.

Uses xinput in order to view key presses, use at own discretion.
The deviceid of the keyboard must be given as an argument to the script. Possible devices can be listed by running xinput.

## Requirments

- xorg-xinput
- mpv

## Example

```
>> xinput 
⎡ Virtual core pointer                    	id=2	[master pointer  (3)]
⎜   ↳ Virtual core XTEST pointer              	id=4	[slave  pointer  (2)]
⎜   ↳ Logitech MX Master 2S                   	id=12	[slave  pointer  (2)]
⎣ Virtual core keyboard                   	id=3	[master keyboard (2)]
    ↳ Virtual core XTEST keyboard             	id=5	[slave  keyboard (3)]
    ↳ Power Button                            	id=6	[slave  keyboard (3)]
    ↳ Logitech MX Master 2S                   	id=17	[slave  keyboard (3)]
    ↳ USB-HID Keyboard                        	id=8	[slave  keyboard (3)]
```

Then running on USB-HID Keyboard with:

`>> ./sudo-gg 8`
