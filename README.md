# Mixxx-Pioneer-DDJ-SB3
Mixxx  controller mappings for the Pioneer DDJ SB3

These files are based on the DDJ-SB2 files that are part of the Mixxx distribution: https://github.com/mixxxdj/mixxx/tree/master/res/controllers, however they where adjusted to work fine with DDJ-SB3

## Other branches
You may want to check the branch [8-hotcues](https://github.com/julia-otran/Mixxx-Pioneer-DDJ-SB3/tree/8-hotcues). The difference is the `HOT CUE` pads: Use the pads as hotcues, and pressing shift:
  - The 4 pads on top will delete hotcues 1-4
  - The 4 pads in bottom will be start, rewind, forward and censor.

The behavior on `master` branch is different:
  - The 4 pads on top are hotcues 1-4, pressing with shift will delete.
  - The 4 pads on bottom are start, rew, forward, censor. Pressing shift will give you hotcues 5-8

## Installing / Updating
- First option: Execute one of the scripts:
  ### Windows
  Just double-click the bat file, it will copy files for you (this is not a virus, it will just copy the files for you, if are feeling unsafe, copy files manualy)
  ```
  install-win.bat
  ```

  ### Linux
  1. Open a terminal
  2. `cd` to the directory where you downloaded / clonned this project
  3. Run `./install-linux.sh`

  ### MacOS
  1. Open a terminal
  2. `cd` to the directory where you downloaded / clonned this project
  3. Run `./install-osx.sh`

- Second option: You can just copy the files
```
lodash.mixxx.js
midi-components-0.0.js
Pioneer-DDJ-SB3-scripts.js
Pioneer-DDJ-SB3.midi.xml
```
to the Mixxx controllers folder.

*Beware: If you are updating, I would recommend that you delete any XML files that contains `DDJ-SB3` and activate your controller again in Mixxx*

## Using Effects
  - The 1, 2, 3 will always turn on/off the effect

  - The `Level` knob will change the effect unit `Master`, IF NONE EFFECT IS SELECTED.

  - Pressing SHIFT + 1, 2 or 3 will SELECT the effect. When there is a selected effect:
    - The `Level` now will change the `META` of the selected effect.

    - Holding SHIFT while changing `GAIN`, one of `EQ` or `FILTER` will change the selected effect params.

    - You can DELESECT it pressing SHIFT and the lighted effect button. After that no buttons will be lighted meaning that no effect if selected


## Midi Message Lists
* Midi Message List for the SB3 (PDF): https://www.pioneerdj.com/-/media/pioneerdj/software-info/controller/ddj-sb3/ddj-sb3_midi_message_list_e1.pdf
* Midi Message List for the SB2 (PDF), for comparison against SB3: http://faq.pioneerdj.com/files/img/DDJ-SB2_List_of_MIDI_Messages_E.pdf

## Running the Tests
1. Install Node
1. Install Yarn
1. Install Jest
1. run yarn test

## Feature Matrix

| Feature      | Deck 1 | Deck 2 | Deck 3 | Deck 4 |
|--------------|--------|--------|--------|--------|
| Play / Pause | Yes    | Yes    | Yes    | Yes    |
| Cue          | Yes    | Yes    | Yes    | Yes    |
| Key Lock     | Yes    | Yes    | Yes    | Yes    |
| Sync         | Yes    | Yes    | Yes    | Yes    |
| Tempo Range  | Yes    | Yes    | Yes    | Yes    |
| Fx           | Yes    | Yes    | Yes    | Yes    |
| Auto Loop    | Yes    | Yes    | Yes    | Yes    |
| Vynil / Slip | Yes    | Yes    | Yes    | Yes    |
| Hotcue       | Yes    | Yes    | Yes    | Yes    |
| Sampler      | Yes    | Yes    | Yes    | Yes    |
| Beat jump    | Yes    | Yes    | Yes    | Yes    |
| Roll         | Yes    | Yes    | Yes    | Yes    |
| Slicer!!!    | Yes    | Yes    | Yes    | Yes    |
| Eq           | Yes    | Yes    | Yes    | Yes    |

*In fact, I think all features are working. Let me know, or open a issue if you experience some problem.*


