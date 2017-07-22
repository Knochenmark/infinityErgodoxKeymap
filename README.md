# Infinity Ergodox Keymap

This is my current Ergodox Keyboard Layout.

The layout uses the base German ISO layout with a some adaptions, since the ergodox lacks a few keys on the base layer.
Noticable is this especially for the umlauts `ä`,`ö` and `ü` and also the `ß` letter. Also the Ergodox lacks keys for the keys next to the umlauts and a key left of `Y` that is used for `<`. Luckily we can create layers.

#Layers

I went with the default 3 base layers for now which are `default`, `symbols` and `media`.

##Default
_ToDo: add default layer description_

##Symbols
_ToDo: add symbol layer description_

##Media
_ToDo: add media layer description_

# Build the QMK firmware

Change `knochenmark` to your own keymap name.

```shell
$ make ergodox-infinity-knochenmark VISUALIZER_ENABLE=yes LCD_BACKLIGHT_ENABLE=yes LCD_ENABLE=yes MASTER=left
```

#Flash it

For the **left** half
```shell
$ sudo make ergodox-infinity-knochenmark-dfu-util
```
For the **right** half
```shell
$ sudo make ergodox-infinity-knochenmark-dfu-util MASTER=right
```

#ToDo's

- Add images of layout using keyboard layouter or the ergodox ez editor
- Test the layout under Windows (might require a seperate Windows layer)
- Consider repositioning of Home/End keys
- Gaming layer with WASD offset by 1 to the right and function keys on base layer
- Print a image of the layout
- Add goals section

#Useful Resources

[Ergodox Infinity LCD Screen Support with QMK](https://www.reddit.com/r/MechanicalKeyboards/comments/6576f8/psa_the_screens_on_the_infinity_ergodox_now_work/)

[Building the QMK Firmware Documentation](https://github.com/qmk/qmk_firmware/tree/master/keyboards/ergodox)

[QMK Keycodes](https://docs.qmk.fm/basic_keycodes.html)
