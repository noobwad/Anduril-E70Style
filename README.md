# Anduril-E70Style

Intended for Noctigon lights with tailswitches, this version of Anduril 2 has been modified to behave like the Acebeam E70. A single press of the button while off will not do anything, which helps prevent accidental activations. Two successive presses of the button are required to turn the light on. Momentary mode has also been removed.

## OPERATION

### While off:
- 2C - Turn light onto memorized level
- 2H - Turn light on to minimum ramp level
- 3C - Turn light on to maximum ramp level
- 3H - Turn light on to Turbo while the button is held down, turn off when released

- 4C - Enter Lockout mode
- 5C - Enter Battery check/utility modes
- 5H - Enter candle/strobe modes

### While on:
- 1C - Turn the light off
- 1H - Ramp up to top of ramp
- 2H - Ramp down to bottom of ramp
- 3H - Activate Turbo while the button is held
- 2C - Jump to Turbo output

The rest of the operation is as normal. Please refer to the official Anduril manual below.

## CUSTOMIZING

### USE THE RIGHT HEX!
There are three hex files in the Hexes directory. Select the appropriate hex for your flashlight configuration.
- `E70Style-nofet.hex` is for all standard KR1 models, and KR4 models with E21A emitters. Recommended also for Nichia 219b emitters if you want to err on the safe side.
- `E70Style-219b.hex` is for the KR4 with Nichia 219b or 219c LEDs. Limits FET to 50% power
- `E70Style-FET.hex` is for all other versions of the KR4, and the SBT90.2 version of the KR1.

### Build Your Own
These are for single-channel configurations. For any custom configuration, download the desired `.h` config file from ToyKepper's flashlight firmware repository. Go to the `main.c` file under the Anduril Code directory and modify line 57 `#define CONFIGFILE` with the intended configuration.

Config files available on the flashlight firmware repository here: https://bazaar.launchpad.net/~toykeeper/flashlight-firmware/trunk/files/head:/ToyKeeper/spaghetti-monster/anduril

## ANDURIL

Manual for use of Anduril:
https://toykeeper.net/torches/fsm/anduril2/anduril-manual.txt

Standard Anduril hex files: https://toykeeper.net/torches/fsm/anduril2/

Use the right hex for your light! 
https://toykeeper.net/torches/fsm/anduril2/MODELS

Guide for reflashing: https://budgetlightforum.com/node/68263


Anduril by ToyKeeper - Source code: https://launchpad.net/flashlight-firmware
