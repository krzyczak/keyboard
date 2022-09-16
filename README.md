# Mechanical Keyboard Specyfication

1. Must support QMK. everything should be the same as https://gitlab.cairn-devices.eu/cairntech/cairn-mesa-key/ regarding firmware
2. Must be RGB
3. All the designs should be based on https://gitlab.cairn-devices.eu/cairntech/cairn-mesa-key/
4. Must use the [MX ULP Tactile](https://www.cherrymx.de/en/cherry-mx/mx-ultra-low-profile/mx-ulp-tactile.html#techSpecs)

The goal is to have a keyboard based on the cairn mesa designs (equally flat, with the same keys and firmware and materials), supporting Cherry [MX ULP Tactile](https://www.cherrymx.de/en/cherry-mx/mx-ultra-low-profile/mx-ulp-tactile.html#techSpecs) switches but to have the same layout as the 2015 Macbook Pro 15" A1398 model.
This layout is almost like 75%, with apple own modification.

Since there is no easy way to find mechanical switches for half the key (like apple top row finction keys and half sized arrow keys), a workaround needs to be put in place:
- arrow keys need a workaround
- the top row can simply be replaced with full size keys

The following picture shows one of the possibilities for this:
<img width="838" alt="Screen Shot 2022-09-15 at 23 43 09" src="https://user-images.githubusercontent.com/38408/190640593-065fa96c-b3c9-48fe-922f-c51f3bc8adb1.png">

The example layout data is in the [example-layout.txt](https://github.com/krzyczak/keyboard/blob/master/example-layout.txt) which can be pasted in the "Raw Data" section on the http://www.keyboard-layout-editor.com/ website to show it.

Obviously, the layout shown there does not take into account the size of the [MX ULP Tactile](https://www.cherrymx.de/en/cherry-mx/mx-ultra-low-profile/mx-ulp-tactile.html#techSpecs) switches, so it should be used as a guide only.

The data sheet for the switch is provided here https://www.cherrymx.de/_Resources/Persistent/8/c/3/4/8c348ad8022fdd2c96033bdb32948fcb036a4ecd/CHERRY_MX_ULP_Tactile_Datasheet.pdf


## Task description
1. Re-design the PCB with KiCad files from the https://gitlab.cairn-devices.eu/cairntech/cairn-mesa-key/-/tree/main/Electronics repository so that it has the apple layout, and all the requirements above. The files should be ready for the https://www.pcbway.com/ to take the order.
2. Produce the specification of what parameters to select when ordering the PCB from pcbway.com
3. Re-design the IGES and Solidworks files from the https://gitlab.cairn-devices.eu/cairntech/cairn-mesa-key/-/tree/main/Mechanics repository for the casing, topsheet and all other parts, so that they fit the new keyboard layout and size. These files should be ready for a CNC company to be able to cut out the needed parts.
