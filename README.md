# Compact Voice Access bar

A [Windhawk](https://windhawk.net/) mod for Windows 11 that turns the
full-width Voice Access bar into a compact window near the top-right corner of
the monitor, and stops it from reserving a strip of the screen. Maximized
windows get the whole screen back.

Mod file: [`voice-access-compact-bar.wh.cpp`](voice-access-compact-bar.wh.cpp)

## Install

Once accepted into the Windhawk catalog, search for **Compact Voice Access bar**
in Windhawk and install it from there.

Until then, or to try a development build:

1. Open Windhawk and click **Explore**, then **Create a new mod**.
2. Replace the editor contents with the mod file from this repository.
3. Click **Compile**.
4. Start Voice Access. The mod attaches a short moment after the bar appears.

Keep Windhawk running while Voice Access is open.

## Settings

| Setting | Default | Meaning |
| --- | --- | --- |
| Compact placement | on | Compact window instead of the full-width docked bar |
| Window width | 900 | Width of the compact window in pixels, at least 300 |
| Distance from top | 100 | Gap between the top of the monitor and the window |

Settings apply immediately. Disabling the mod, or turning compact placement
off, restores the original bar and its reserved strip.

## Notes

* Only the outer Voice Access window is resized. Voice Access lays out the
  bar contents itself, so a very narrow width may clip controls.
* The mod attaches once per Voice Access launch. If Voice Access recreates
  its bar after a display change, restart Voice Access.
* Enable Windhawk logging for the mod to see the attach step and every
  window position and work-area change it applies.

## License

[MIT](LICENSE)
