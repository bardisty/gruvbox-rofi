# gruvbox-rofi

> Gruvbox dark and light themes for Rofi

Rofi color themes based on the
[Gruvbox color scheme](https://github.com/morhetz/gruvbox).

Includes six versions to choose from:

- __[Gruvbox Dark](gruvbox-dark.theme)__
  - [Gruvbox Dark (soft contrast)](gruvbox-dark-soft.theme)
  - [Gruvbox Dark (hard contrast)](gruvbox-dark-hard.theme)
- __[Gruvbox Light](gruvbox-light.theme)__
  - [Gruvbox Light (soft contrast)](gruvbox-light-soft.theme)
  - [Gruvbox Light (hard contrast)](gruvbox-light-hard.theme)

## Dark

![gruvbox dark theme screenshot](docs/gruvbox-dark.png "gruvbox dark theme")

### Soft Contrast

![gruvbox dark theme (soft contrast) screenshot](docs/gruvbox-dark-soft.png "gruvbox dark theme (soft contrast)")

### Hard Contrast

![gruvbox dark theme (hard contrast) screenshot](docs/gruvbox-dark-hard.png "gruvbox dark theme (hard contrast)")

## Light

![gruvbox light theme screenshot](docs/gruvbox-light.png "gruvbox light theme")

### Soft Contrast

![gruvbox light theme (soft contrast) screenshot](docs/gruvbox-light-soft.png "gruvbox light theme (soft contrast)")

### Hard Contrast

![gruvbox light theme (hard contrast) screenshot](docs/gruvbox-light-hard.png "gruvbox light theme (hard contrast)")

## Installation

1. [Download](https://github.com/bardisty/gruvbox-rofi/archive/master.zip)
   or clone the repository:

   `git clone https://github.com/bardisty/gruvbox-rofi`

2. Edit your `~/.Xresources` file and include one of the themes:

   ```xdefaults
   #include /home/user/path/to/gruvbox-dark.theme
   ```

3. Merge your edited `.Xresources` file with `xrdb`:

   `xrdb -merge ~/.Xresources`

### Example Install

The following commands will install the dark theme:

1. `mkdir -p ~/.Xresources.d/rofi/themes/gruvbox`
- `git clone https://github.com/bardisty/gruvbox-rofi ~/.Xresources.d/rofi/themes/gruvbox`
- `echo '#include "/home/your-user/.Xresources.d/rofi/themes/gruvbox/gruvbox-dark.theme"' >> ~/.Xresources`
- `xrdb -merge ~/.Xresources`

*Be sure to replace `your-user` in step 3 with the name of your user.*

## Links

- [Rofi](https://github.com/DaveDavenport/rofi) window switcher, run dialog,
  and dmenu replacement
- [Gruvbox](https://github.com/morhetz/gruvbox) color scheme for Vim

## License

[MIT](LICENSE)
