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

![](screenshots/fallen-leaves.png)

[`pixel-themes-gray-weather`](https://lospec.com/palette-list/gray-weather)

![](screenshots/gray-weather.png)

[`pixel-themes-steam-lords`](https://lospec.com/palette-list/steam-lords)

![](screenshots/steam-lords.png)

[`pixel-themes-psygnosia`](https://lospec.com/palette-list/psygnosia)

![](screenshots/psygnosia.png)

[`pixel-themes-miri16`](https://lospec.com/palette-list/miri16)

![](screenshots/miri16.png)

[`pixel-themes-alia16`](https://lospec.com/palette-list/alia16)

![](screenshots/alia16.png)

## TODO

- [X] Dark themes
- [ ] Light themes
