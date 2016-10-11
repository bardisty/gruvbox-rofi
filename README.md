# gruvbox-rofi

> Gruvbox dark and light themes for Rofi

## Dark

![gruvbox dark theme screenshot](docs/gruvbox-dark.png "gruvbox dark theme")

## Light

![gruvbox light theme screenshot](docs/gruvbox-light.png "gruvbox light theme")

## Installation

1. [Download](https://github.com/bardisty/gruvbox-rofi/archive/master.zip)
   or clone the repository:

   `git clone https://github.com/bardisty/gruvbox-rofi`

2. Edit your `~/.Xresources` file and include one of the two themes:

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

To install the light theme instead, replace step 3 with:

`echo '#include "/home/your-user/.Xresources.d/rofi/themes/gruvbox/gruvbox-light.theme"' >> ~/.Xresources`

*Be sure to replace `your-user` in step 3 with the name of your user.*

## Links

- [Rofi](https://github.com/DaveDavenport/rofi) window switcher, run dialog,
  and dmenu replacement
- [Gruvbox](https://github.com/morhetz/gruvbox) color scheme for Vim

## License

[MIT](LICENSE)
