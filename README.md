# Keyboards


## YMD40 (the "lego keyboard")

The v1 of [this keyboard off AliExpress](https://www.aliexpress.com/item/32821953148.html?gatewayAdapt=glo2bra), that has a slightly larger spacebar. Nicknamed the "lego keyboard" by my mom. [Here](https://drive.google.com/file/d/1h5RA14a_WeWlXNpFgBsr-QJrQNSs6d7s/view) is the user manual.

<img src="https://github.com/sofiafrocha/keyboards/blob/main/images/keyboard-lego-layers.png?raw=true" alt="keymap of ymd40 keyboard" style="zoom: 67%;" />

### Features
- Two layers (one with most used letters and a second one with numbers, symbols, light controls and media playback)
- Auto-shift if you hold a key (minimizes pain on the pinky finger)
- Made to be used with the Portuguese layout to let me write special characters (like ç, é, ã, ê)

### How to edit the keymap
1. Load `sofia.json` on [QMK Configurator](https://config.qmk.fm/#/amjkeyboard/amj40/LAYOUT_ortho_275u_space)
2. Download the new `.json` file into `qmk_firmware` folder
3. Run `qmk json2c sofia.json`

### How to compile
1. Install [QMK Firmware](https://docs.qmk.fm/#/newbs_getting_started)
2. Put the `ymd40` folder inside the `qmk_firmware/keyboards/amj40/keymaps` folder and rename it to `sofia`
3. Run `qmk compile -kb amjkeyboard/amj40 -km sofia`
4. Use the `.hex` file to flash the keyboard using [QMK Toolbox](https://github.com/qmk/qmk_toolbox) (select the `atmega32u4` controller)


## ZSA Moonlander

The [Moonlander](https://www.zsa.io/moonlander/) is a split, ergonomic, ortho keyboard.

<img src="https://github.com/sofiafrocha/keyboards/blob/main/images/moonlander-layer-1.png?raw=true" alt="keymap of ymd40 keyboard" style="zoom: 67%;" />
<img src="https://github.com/sofiafrocha/keyboards/blob/main/images/moonlander-layer-2.png?raw=true" alt="keymap of ymd40 keyboard" style="zoom: 67%;" />

### Features
- Two layers (one with most used letters, numbers and symbols and a second one with light controls and media playback)
- Auto-shift if you hold a key (minimizes pain on the pinky finger)
- Made to be used with the Portuguese layout to let me write special characters (like ç, é, ã, ê)


## How to edit

1. Edit the config using [Oryx](https://configure.zsa.io/moonlander/layouts/BO6KW/latest/0)


## How to compile

1. Download [Wally](https://www.zsa.io/wally/)
2. Use the `.hex` file to flash the board


# Contra

This [Contra](https://www.40percent.club/2018/03/contra.html) was a hand-me-down from a coworker that built this keyboard but wasn't a fan of the 40% layout. It's very light and has a very similar keymap to the "lego keyboard".

<img src="https://github.com/sofiafrocha/keyboards/blob/main/images/keyboard-contra-layers.png?raw=true" alt="keymap of ymd40 keyboard" style="zoom: 67%;" />

### How to edit the keymap
1. Load `contra/sofia.json` on [QMK Configurator](https://config.qmk.fm/#/amjkeyboard/amj40/LAYOUT_ortho_275u_space)
2. Download the new `.json` file into `qmk_firmware` folder
3. Run `qmk json2c sofia.json`

### How to compile
1. Install [QMK Firmware](https://docs.qmk.fm/#/newbs_getting_started)
2. Put the `contra` folder inside the `qmk_firmware/keyboards/contra/keymaps` folder and rename it to `sofia`
3. Run `qmk compile -kb contra -km sofia`
4. Use the `.hex` file to flash the keyboard using [QMK Toolbox](https://github.com/qmk/qmk_toolbox) (select the `atmega32u4` controller)
