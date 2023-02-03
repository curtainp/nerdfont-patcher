# nerdfont-patcher
Patcher from [font-patcher](https://github.com/curtainp/nerdfont-patcher.git), and extract the
`glyphs` separately, which convenient for patcher own font.

## Usage
```shell
fontforge -script font-patcher [PATH_TO_FONT]
```

```shell
Nerd Fonts Patcher v2.3.3 (3.5.3) (ff 20230101) executing
usage: font-patcher [-h] [-v] [-s] [-l] [-q] [-w] [-c] [--careful]
                    [--removeligs] [--postprocess [POSTPROCESS]]
                    [--configfile [CONFIGFILE]] [--custom [CUSTOM]]
                    [-ext [EXTENSION]] [-out [OUTPUTDIR]]
                    [--glyphdir [GLYPHDIR]] [--makegroups]
                    [--variable-width-glyphs]
                    [--progressbars | --no-progressbars] [--also-windows]
                    [--fontawesome] [--fontawesomeextension] [--fontlogos]
                    [--octicons] [--codicons] [--powersymbols] [--pomicons]
                    [--powerline] [--powerlineextra] [--material] [--weather]
                    font

Nerd Fonts Font Patcher: patches a given font with programming and development related glyphs

* Website: https://www.nerdfonts.com
* Version: 2.3.3
* Development Website: https://github.com/ryanoasis/nerd-fonts
* Changelog: https://github.com/ryanoasis/nerd-fonts/blob/-/changelog.md

positional arguments:
  font                  The path to the font to patch (e.g., Inconsolata.otf)

options:
  -h, --help            show this help message and exit
  -v, --version         show program's version number and exit
  -s, --mono, --use-single-width-glyphs
                        Whether to generate the glyphs as single-width not double-width (default is double-width)
  -l, --adjust-line-height
                        Whether to adjust line heights (attempt to center powerline separators more evenly)
  -q, --quiet, --shutup
                        Do not generate verbose output
  -w, --windows         Limit the internal font name to 31 characters (for Windows compatibility)
  -c, --complete        Add all available Glyphs
  --careful             Do not overwrite existing glyphs if detected
  --removeligs, --removeligatures
                        Removes ligatures specificed in JSON configuration file
  --postprocess [POSTPROCESS]
                        Specify a Script for Post Processing
  --configfile [CONFIGFILE]
                        Specify a file path for JSON configuration file (see sample: src/config.sample.json)
  --custom [CUSTOM]     Specify a custom symbol font. All new glyphs will be copied, with no scaling applied.
  -ext [EXTENSION], --extension [EXTENSION]
                        Change font file type to create (e.g., ttf, otf)
  -out [OUTPUTDIR], --outputdir [OUTPUTDIR]
                        The directory to output the patched font file to
  --glyphdir [GLYPHDIR]
                        Path to glyphs to be used for patching
  --makegroups          Use alternative method to name patched fonts (experimental)
  --variable-width-glyphs
                        Do not adjust advance width (no "overhang")
  --progressbars        Show percentage completion progress bars per Glyph Set
  --no-progressbars     Don't show percentage completion progress bars per Glyph Set
  --also-windows        Create two fonts, the normal and the --windows version

Symbol Fonts:
  --fontawesome         Add Font Awesome Glyphs (http://fontawesome.io/)
  --fontawesomeextension
                        Add Font Awesome Extension Glyphs (https://andrelzgava.github.io/font-awesome-extension/)
  --fontlogos, --fontlinux
                        Add Font Logos Glyphs (https://github.com/Lukas-W/font-logos)
  --octicons            Add Octicons Glyphs (https://octicons.github.com)
  --codicons            Add Codicons Glyphs (https://github.com/microsoft/vscode-codicons)
  --powersymbols        Add IEC Power Symbols (https://unicodepowersymbol.com/)
  --pomicons            Add Pomicon Glyphs (https://github.com/gabrielelana/pomicons)
  --powerline           Add Powerline Glyphs
  --powerlineextra      Add Powerline Glyphs (https://github.com/ryanoasis/powerline-extra-symbols)
  --material, --materialdesignicons, --mdi
                        Add Material Design Icons (https://github.com/templarian/MaterialDesign)
  --weather, --weathericons
                        Add Weather Icons (https://github.com/erikflowers/weather-icons)
```
