# ergodox-infinity-keymap

1. Clone [https://github.com/qmk/qmk_firmware](qmk_firmware) `git clone git@github.com:qmk/qmk_firmware.git`
2. Move into the qmk_firmware directory `cd qmk_firmware`
2. Install dependencies: `./util/install/debian.sh` (for debian)
3. Install qmk: `sudo python3 -m pip install qmk`
4. Clone this repo into `git clone git@github.com:MarkHedleyJones/ergodox-infinity-keymap.git keyboards/input_club/ergodox_infinity/keymaps/my-custom-keymaps`
6. Generate keymap source file `qmk json2c keyboards/input_club/ergodox_infinity/keymaps/my-custom-keymaps/keymap.json > keyboards/input_club/ergodox_infinity/keymaps/my-custom-keymaps/keymap.c`
8. Compile and program left side `sudo make input_club/ergodox_infinity:my-custom-keymaps:dfu-util-split-left`
9. Compile and program right side `sudo make input_club/ergodox_infinity:my-custom-keymaps:dfu-util-split-right`
