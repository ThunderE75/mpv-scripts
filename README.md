# MPV Scripts

## Script Breakdown

- [autoload](./scripts/autoload.lua) - [[source]()] - This script automatically loads playlist entries before and after the currently played file. 
- [autosub](./scripts/) - [[source](https://github.com/davidde/mpv-autosub)] - This script uses Subliminal to download subtitles.
- [blackout](./scripts/blackout.lua) - [[source](https://github.com/sibwaf/mpv-scripts/blob/master/blackout.lua)] - Turns the screen completely black and pauses on a button press ([b] by default)
- [delete_file](./scripts/delete_file.lua) - [[source](https://github.com/zenyd/mpv-scripts/blob/master/delete_file.lua)] - This script is used to delete files.
- [mpv-menu-plugin](./scripts/) - [[source](https://github.com/tsl0922/mpv-menu-plugin)] - Configurable context menu for mpv on Windows, with additional support for native file dialog and clipboard.
- [ModernX](./scripts/modernx.lua) - [[source](https://github.com/cyl0/ModernX)] - An MPV OSC script based on [mpv-osc-modern](https://github.com/maoiscat/mpv-osc-modern/) that aims to mirror the functionality of MPV's stock OSC while with a more modern-looking interface.
- [pause-when-minimize](./scripts/pause-when-minimize.lua) - [[source](https://github.com/mpv-player/mpv/blob/master/TOOLS/lua/pause-when-minimize.lua)] - This script pauses playback when minimizing the window, and resumes playback.
- [playlistmanager](./scripts/playlistmanager.lua) - [[source](https://github.com/jonniek/mpv-playlistmanager)] - This script allows you to see and interact with your playlist in an intuitive way.
- [thumbfast](./scripts/thumbfast.lua) - [[source](https://github.com/po5/thumbfast)] - High-performance on-the-fly thumbnailer script for mpv
- [mpv-pointer-event](./scripts/pointer-event.lua) - [[source](https://github.com/christoph-heinrich/mpv-pointer-event)] - Mouse/Touch input event detection for mpv.
- [touch-gestures](./scripts/touch-gestures.lua) - [[source](https://github.com/christoph-heinrich/mpv-touch-gestures)] - Touch gestures for mpv.

## Fonts

- [Material Design Iconic Font](https://zavoloklom.github.io/material-design-iconic-font/) - Material Design Iconic Font is a full suite of material design icons (used for Modern X OSC)
- [Space Grotesk](https://fonts.google.com/specimen/Space+Grotesk) & [Atkinson Hyperlegible](https://fonts.google.com/specimen/Atkinson+Hyperlegible) - My preferred font for subtitles.

## Installing (Windows)  

1. Navigate to `%APPDATA%` by using the run menu `Win + r`

1. Cloning the repository

    ```git 
    git clone https://github.com/ThunderE75/mpv-scripts mpv
    ```
1. Download Subliminal (for autosub.lua)

   ```
   pip install subliminal
   ```

## Key Bindings


| Key Bind             | Effect                                     |
| -------------------- | ------------------------------------------ |
| `b`                  | blackout (black screen)                    |
| `ctrl + DEL`         | mark/unmark file to be deleted             |
| `alt + DEL`          | show the list of files marked for deletion |
| `ctrl + shift + DEL` | clear the list of marked files             |

> Files will be deleted upon exit [more info](https://github.com/zenyd/mpv-scripts/tree/master?tab=readme-ov-file#delete-file).