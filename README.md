# pixel-themes

Lospec pixel art palettes adapted for Emacs, based on modus-themes.

## Requirements
- Emacs 28.1+
- modus-themes 5.0.0+

## Installation

### Elpaca

```elisp
(use-package pixel-themes
  :ensure (:host github :repo "lucasobx/pixel-themes")
  :config
  (pixel-themes-mode 1)
  (pixel-themes-load-theme 'pixel-themes-miri16))
```

### Manual

Clone the repository and add it to your load path:

```elisp
(use-package pixel-themes
  :ensure nil
  :load-path "~/.config/emacs/themes/pixel-themes"
  :config
  (pixel-themes-mode 1)
  (pixel-themes-load-theme 'pixel-themes-miri16))
```

## Usage

`pixel-themes-mode` adds all pixel themes to the standard Modus Themes commands:

- `pixel-themes-rotate` - cycle through themes
- `pixel-themes-select` - pick a theme interactively
- `pixel-themes-load-random-dark` - load a random dark theme
- `pixel-themes-list-colors-current` - inspect the active theme's palette

### Palette overrides

Each theme exposes a customization variable for palette overrides:

```elisp
(setq pixel-themes-alia16-palette-overrides
      '((bg-main "#0a0a0c")
        (comment green-faint)))
```


## Themes

[`pixel-themes-fallen-leaves`](https://lospec.com/palette-list/twelve-fallen-leaves)

<img width="2560" height="1550" alt="fallen-leaves" src="https://github.com/user-attachments/assets/3670335e-3824-42e9-9eba-8a89fc274c46" />

[`pixel-themes-gray-weather`](https://lospec.com/palette-list/gray-weather)

<img width="2560" height="1550" alt="gray-weather" src="https://github.com/user-attachments/assets/14c75f52-e95e-428b-8314-16c509b8952d" />

[`pixel-themes-steam-lords`](https://lospec.com/palette-list/steam-lords)

<img width="2560" height="1550" alt="steam-lords" src="https://github.com/user-attachments/assets/fe82bee0-472c-4979-977f-fc0b853533c6" />

[`pixel-themes-psygnosia`](https://lospec.com/palette-list/psygnosia)

<img width="2560" height="1550" alt="psygnosia" src="https://github.com/user-attachments/assets/7c30b1ef-0ec6-448f-b31a-951807458958" />

[`pixel-themes-miri16`](https://lospec.com/palette-list/miri16)

<img width="2560" height="1550" alt="miri16" src="https://github.com/user-attachments/assets/e07c3602-eb53-4de0-a9d4-22a1a75e7fca" />

[`pixel-themes-alia16`](https://lospec.com/palette-list/alia16)

<img width="2560" height="1550" alt="alia16" src="https://github.com/user-attachments/assets/d0092545-e1ba-4d9d-acc6-6ffbd3f8d1f4" />

## TODO

- [ ] Light themes
