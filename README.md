# ANSI to HTML command line

## Installation
`npm install -g ansi2html-cli`

## Basic usage
`cat foo.log | ansi2html > foo.html`

## Usage
    ansi2html [-h] [-v] [-f BG] [-b FG] [-s STYLE] [--linebreak] [--no-escape] [--no-wrap]

    Converts piped ansi to html using rburns's ansi-to-html. Intended for use in
    a unix pipeline. e.g. `cat foo.log | ansi2html > foo.html`

    Optional arguments:
      -h, --help            Show this help message and exit.
      -v, --version         Show program's version number and exit.
      -f BG, --foreground BG
                            Default foreground color used when reset codes are
                            encountered (e.g #000).
      -b FG, --background FG
                            Default background color used when reset codes are
                            encountered (e.g #fff).
      -s STYLE, --style STYLE
                            Styles to add to the document (e.g. "font-weight:
                            bold; font-family: monospace;" ).
      --linebreak           Insert <br/> at the end of each line (generally not
                            necessary as we use white-space:pre by default).
      --no-escape           Do not escape XML entities.
      --no-wrap             Do not add wrapping html tags.

## credit to
https://www.npmjs.com/package/ansi-to-html
