# MPV Scripts

This repository contains my MPV Configs, Scripts & Keybinds. This was setup on Windows 11, so some changes might be necessary (Like file paths & cli commands) to make it work on Linux/MacOS.

## Script Breakdown

- [autoload](./scripts/autoload.lua) - [[source](https://github.com/mpv-player/mpv/blob/master/TOOLS/lua/autoload.lua)] - This script automatically loads playlist entries before and after the currently played file. 
- [autosub](./scripts/) - [[source](https://github.com/davidde/mpv-autosub)] - This script uses Subliminal to download subtitles.
- [blackout](./scripts/blackout.lua) - [[source](https://github.com/sibwaf/mpv-scripts/blob/master/blackout.lua)] - Turns the screen completely black and pauses on a button press ([b] by default)
- [delete_file](./scripts/delete_file.lua) - [[source](https://github.com/zenyd/mpv-scripts/blob/master/delete_file.lua)] - This script is used to delete files.
- [mpv-menu-plugin](./scripts/) - [[source](https://github.com/tsl0922/mpv-menu-plugin)] - Configurable context menu for mpv on Windows, with additional support for native file dialog and clipboard.
- [ModernZ](./scripts/modernz.lua) - [[source](https://github.com/Samillion/ModernZ/)] - A fork of ModernX, with build in support for interactive menus & better UI customization. 
- [pause-when-minimize](./scripts/pause-when-minimize.lua) - [[source](https://github.com/mpv-player/mpv/blob/master/TOOLS/lua/pause-when-minimize.lua)] - This script pauses playback when minimizing the window, and resumes playback.
- [playlistmanager](./scripts/playlistmanager.lua) - [[source](https://github.com/jonniek/mpv-playlistmanager)] - This script allows you to see and interact with your playlist in an intuitive way.
- [thumbfast](./scripts/thumbfast.lua) - [[source](https://github.com/po5/thumbfast)] - High-performance on-the-fly thumbnailer script for mpv
- [mpv-pointer-event](./scripts/pointer-event.lua) - [[source](https://github.com/christoph-heinrich/mpv-pointer-event)] - Mouse/Touch input event detection for mpv.
- [touch-gestures](./scripts/touch-gestures.lua) - [[source](https://github.com/christoph-heinrich/mpv-touch-gestures)] - Touch gestures for mpv.
- [mpv-gallery-view](./scripts/playlist-view.lua) [[source](https://github.com/occivink/mpv-gallery-view)] - Playlist grid view
- [mpv-gallery-view (Contact Sheet)](./scripts/contact-sheet.lua) [[source](https://github.com/occivink/mpv-gallery-view)] - Contact sheet view

## Fonts

- [Space Grotesk](https://fonts.google.com/specimen/Space+Grotesk) & [Atkinson Hyperlegible](https://fonts.google.com/specimen/Atkinson+Hyperlegible) - My preferred font for subtitles.
- [Fluent System Icons](https://github.com/microsoft/fluentui-system-icons) - A modified version by [Xurdejl](https://github.com/Xurdejl) for use on (ModernZ OSC)
- [Material Design Iconic](https://github.com/Samillion/ModernZ/blob/main/material-design-icons.ttf) - Material Design Icons used for ModernZ OSC

## Installing (Windows)  

> Prerequisites - [mpv](https://mpv.io/installation/), [git](https://git-scm.com/) & [python (pip)](https://www.python.org/downloads/).

1. Navigate to `%APPDATA%` by using the run menu `Win + r`

2. Cloning the repository

    ```git 
    git clone https://github.com/ThunderE75/mpv-scripts mpv
    ```
3. Download Subliminal (for [autosub.lua](./scripts/autosub.lua))

   ```
   pip install subliminal
   ```

## Key Bindings

| Key Bind             | Description                                                |
| -------------------- | ---------------------------------------------------------- |
| `b`                  | blackout (black screen)                                    |
| `Keypad <x>`         | Seek to `x*10%` (Youtube-esque seek)                       |
| `Ctrl + ALT + s`     | Download Subtitles                                         |
| `SHIFT + Enter`      | Show playlist manager console                              |
| `SHIFT + ALT + s`    | Cycle Playlist Sort                                        |
| `SHIFT + ALT + h`    | Shuffle current playlist                                   |
| `Ctrl + DEL`         | Mark/Unmark file to be deleted                             |
| `ALT + DEL`          | Show the list of files marked for deletion                 |
| `Ctrl + SHIFT + DEL` | Clear the list of marked files (files will not be deleted) |

> Files will be deleted only upon exit [more info](https://github.com/zenyd/mpv-scripts/tree/master?tab=readme-ov-file#delete-file).

### Some Default Key binds 

| Key Bind        | Description      |
| --------------- | ---------------- |
| `PGUP` or `@`   | Next Chapter     |
| `PGDOWN` or `!` | Previous Chapter |
