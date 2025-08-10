# A minimalist userChrome.css

`userChrome.css` is a Firefox configuration file which allows the user to
define his own look of the browser.

This particular config works best with a minimalist WM like dwm, xmonad or
awesome.

## How to use

Enable user chrome:

1) in `about:config` set `toolkit.legacyUserProfileCustomizations.stylesheets` to `true`

Enable compact mode:

1) in `about:config` set `browser.compactmode.show` to `true`
2) in the customize toolbar menu set `density` to `compact`

Via the customize toolbar menu remove firefox view (the top-left corner icon)

Enable dark theme in settings.

Copy `userChrome.css` to the `chrome` directory in your firefox profile. If
there is no such directory create it.

If you're unsure what the path to your profile's directory is, you can find out
by going to `about:profiles`.

I use [Vimium C](https://addons.mozilla.org/en-US/firefox/addon/vimium-c/), you can use [tridactyl](https://github.com/tridactyl/tridactyl) or a
similar extension for best results.

Color of text in a tab is determined by its container. If a tab has no
container, fallback colors are used. You can change the basic colorscheme by
adjusting values of variables defined at the top of `userChrome.css`.

## Screenshots

o
With navbar shown:

o
## Common issues

### black stripe under tab bar

Increase the value of the `--tab-min-height` variable in `userChrome.css`.

### I want to disable favicons

Search for 'disable favicons' and uncomment the relevant line.

## Credit

This userchrome is a fork of
[aadilayub's](https://github.com/aadilayub/firefox-i3wm-theme).
