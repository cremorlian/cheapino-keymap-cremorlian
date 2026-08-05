# cheapino-keymap-cremorlian

Custom QMK keymap for the [Cheapino](https://github.com/tompi/qmk_firmware/tree/master/keyboards/cheapino) split keyboard. Optimised for QWERTY, vi, and CLI usage.

## Setup

This repo is designed to live outside the QMK firmware tree and be symlinked in:

```
/path/to/cheapino-keymap-cremorlian/   (this repo)
    ↳ symlinked to
/path/to/qmk_firmware/keyboards/cheapino/keymaps/cremorlian
```

### Creating the symlink

```bash
ln -s /path/to/cheapino-keymap-cremorlian \
  /path/to/qmk_firmware/keyboards/cheapino/keymaps/cremorlian
```

### Building

```bash
qmk compile -kb cheapino -km cremorlian
```

### Flashing

```bash
qmk flash -kb cheapino -km cremorlian
```

## Project structure

```
.
├── keymap.json          # QMK keymap (QMK Configurator format)
├── config.h             # QMK config (Chordal Hold, mouse settings)
├── LICENSE
└── README.md
```
