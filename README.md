# ergodox-infinity-keymap

This repository contains the layout files for my Ergodox Infinity keyboard.
It has the Colemak layout on the base layer, Colemak Mod-DH on the second layer (something I trying out), and custom overlays for navigation/programming/data-entry.

![Ergodox Infinity](https://massdrop-s3.imgix.net/product-images/infinity-ergodox/MD-15095_20160131210416_786e0e40ad513ac0.jpg?bg=f0f0f0)

## Flashing setup (one-time)

1. Clone [https://github.com/qmk/qmk_firmware](qmk_firmware) `git clone git@github.com:qmk/qmk_firmware.git`
1. Move into the qmk_firmware directory `cd qmk_firmware`
1. Install dependencies: `./util/install/debian.sh` (for debian)
1. Install qmk: `sudo python3 -m pip install qmk`
1. Clone this repo into `git clone git@github.com:MarkHedleyJones/ergodox-infinity-keymap.git keyboards/input_club/ergodox_infinity/keymaps/my-custom-keymaps`

## Updating (repeatable)
1. Visit [config.qmk.fm](https://config.qmk.fm/#/input_club/ergodox_infinity/LAYOUT_ergodox), click upload and supply the keymap.json file in this repository.
1. Modify and re-upload the keymap.json file.
1. Generate keymap source file `qmk json2c keyboards/input_club/ergodox_infinity/keymaps/my-custom-keymaps/keymap.json > keyboards/input_club/ergodox_infinity/keymaps/my-custom-keymaps/keymap.c`
1. Compile and program left side `sudo make input_club/ergodox_infinity:my-custom-keymaps:dfu-util-split-left`
1. Compile and program right side `sudo make input_club/ergodox_infinity:my-custom-keymaps:dfu-util-split-right`


# Current keymap:

<!-- Insert layer_0.png image -->
[![Layer 0](https://raw.githubusercontent.com/MarkHedleyJones/ergodox-infinity-keymap/master/layer_0.png)](https://raw.githubusercontent.com/MarkHedleyJones/ergodox-infinity-keymap/master/layer_0.png)

 <!-- Insert layer_1.png image -->
[![Layer 1](https://raw.githubusercontent.com/MarkHedleyJones/ergodox-infinity-keymap/master/layer_1.png)](https://raw.githubusercontent.com/MarkHedleyJones/ergodox-infinity-keymap/master/layer_1.png)

 <!-- Insert layer_2.png image -->
[![Layer 2](https://raw.githubusercontent.com/MarkHedleyJones/ergodox-infinity-keymap/master/layer_2.png)](https://raw.githubusercontent.com/MarkHedleyJones/ergodox-infinity-keymap/master/layer_2.png)

 <!-- Insert layer_3.png image -->
[![Layer 3](https://raw.githubusercontent.com/MarkHedleyJones/ergodox-infinity-keymap/master/layer_3.png)](https://raw.githubusercontent.com/MarkHedleyJones/ergodox-infinity-keymap/master/layer_3.png)
