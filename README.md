# gruvbox-rofi

> Gruvbox dark and light color themes for Rofi

[Rofi](https://github.com/DaveDavenport/rofi) color themes based on the
[Gruvbox color scheme](https://github.com/morhetz/gruvbox).

Includes six versions to choose from:

- __[Gruvbox Dark](#dark-gruvbox-darktheme)__
  - [Gruvbox Dark (soft contrast)](#dark-soft-contrast-gruvbox-dark-softtheme)
  - [Gruvbox Dark (hard contrast)](#dark-hard-contrast-gruvbox-dark-hardtheme)
- __[Gruvbox Light](#light-gruvbox-lighttheme)__
  - [Gruvbox Light (soft contrast)](#light-soft-contrast-gruvbox-light-softtheme)
  - [Gruvbox Light (hard contrast)](#light-hard-contrast-gruvbox-light-hardtheme)

## Screenshots

### Dark ([`gruvbox-dark.theme`](gruvbox-dark.theme))

![gruvbox dark theme screenshot](docs/gruvbox-dark.png "gruvbox dark theme")

#### Dark (soft contrast) ([`gruvbox-dark-soft.theme`](gruvbox-dark-soft.theme))

![gruvbox dark theme (soft contrast) screenshot](docs/gruvbox-dark-soft.png "gruvbox dark theme (soft contrast)")

#### Dark (hard contrast) ([`gruvbox-dark-hard.theme`](gruvbox-dark-hard.theme))

![gruvbox dark theme (hard contrast) screenshot](docs/gruvbox-dark-hard.png "gruvbox dark theme (hard contrast)")

### Light ([`gruvbox-light.theme`](gruvbox-light.theme))

![gruvbox light theme screenshot](docs/gruvbox-light.png "gruvbox light theme")

#### Light (soft contrast) ([`gruvbox-light-soft.theme`](gruvbox-light-soft.theme))

![gruvbox light theme (soft contrast) screenshot](docs/gruvbox-light-soft.png "gruvbox light theme (soft contrast)")

#### Light (hard contrast) ([`gruvbox-light-hard.theme`](gruvbox-light-hard.theme))

![gruvbox light theme (hard contrast) screenshot](docs/gruvbox-light-hard.png "gruvbox light theme (hard contrast)")

## Installation

These themes are included with Rofi as of version
[1.3.0](https://github.com/DaveDavenport/rofi/releases/tag/1.3.0). Run
`rofi-theme-selector` to preview/apply them with Rofi's theme selector
script.

See [Manual Installation](#manual-installation) if you wish to install the
themes manually. This may be preferable if you plan on customizing them.
See also [Customization](#customization).

### Manual Installation

1. [Download](https://github.com/bardisty/gruvbox-rofi/archive/master.zip)
   or clone the repository:

   `git clone https://github.com/bardisty/gruvbox-rofi`

2. Edit your Rofi configuration file (`~/.config/rofi/config`) and include
   one of the themes:

   ```xdefaults
   #include /home/user/path/to/gruvbox-dark.theme
   ```

#### Example Install

The following commands will install the dark theme. *Replace `your-user` in
the last step with your system user account name.*

1. `mkdir -p ~/.config/rofi/themes/gruvbox`
- `git clone https://github.com/bardisty/gruvbox-rofi ~/.config/rofi/themes/gruvbox`
- `echo '#include "/home/your-user/.config/rofi/themes/gruvbox/gruvbox-dark.theme"' >> ~/.config/rofi/config`

## Customization

Customization can be done a few ways:
- Edit a `.theme` file directly, or make a copy of the `.theme` file and
  edit that (see [Manual Installation](#manual-installation))
- Copy the contents of a `.theme` file into your Rofi configuration file
  (`~/.config/rofi/config`) and modify it there
- Apply a theme with `rofi-theme-selector` or add it to the Rofi
  configuration file manually (see [Manual Installation](#manual-installation)),
  then add your overrides under the `#include` line, for example:

  ```xdefaults
  ! Gruvbox color scheme
  #include "/home/user/.config/rofi/themes/gruvbox-dark.theme"

  ! gruvbox-dark.theme: green for active row background colors (default: yellow)
  !                  bg       fg       bg-alt   hl-bg,   hl-fg
  rofi.color-active: #98971a, #282828, #98971a, #b8bb26, #282828
  ```

The last option is ideal if you only want to change a setting or two, such
as the active row colors or the border color. It also allows you to easily
remain updated with the upstream versions of the themes.

## Links

- [Rofi](https://github.com/DaveDavenport/rofi) window switcher, run
  launcher, ssh dialog, and dmenu replacement
- [Gruvbox](https://github.com/morhetz/gruvbox) color scheme for Vim

## License

[MIT](LICENSE)
