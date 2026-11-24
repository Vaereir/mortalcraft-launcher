# Mortalcraft

Mortalcraft is a World of Warcraft 3.3.5a server that is being tested. You can only play if you were invited.

## What you need

- An invitation: an account name, a password and the server's address.
- Your own copy of World of Warcraft 3.3.5a (build 12340, English). Use a separate copy for Mortalcraft, because
  its files change the game.

## Getting started

1. Download `Mortalcraft-Launcher.exe` from the [latest release](../../releases/latest).
2. Put it in your game folder, next to `Wow.exe`, and start it. Windows will say it doesn't know who made it:
   choose "More info", then "Run anyway".
3. Type the server address you were given and press Play.
4. Log in with your account name and password.

Always start the game with the launcher. It keeps your files up to date and points the game at the server.

## On Linux

The game is a Windows program, so on Linux it runs through Wine. The Linux launcher does everything the Windows one
does and starts the game through Wine for you.

1. Install Wine and the web view the launcher's window needs, from your system's software store or with one of
   these commands in a terminal:
   - Ubuntu, Linux Mint, Pop!_OS, Debian: `sudo dpkg --add-architecture i386 && sudo apt update && sudo apt install wine wine32 libwebkit2gtk-4.1-0`
   - Fedora: `sudo dnf install wine webkit2gtk4.1`
   - Arch, Manjaro, SteamOS desktop: `sudo pacman -S wine webkit2gtk-4.1`
2. Download `Mortalcraft-Launcher-Linux` from the [latest release](../../releases/latest) and put it in your game
   folder, next to `Wow.exe`.
3. Let it run as a program: right-click it, open Properties, and on the Permissions tab tick "Allow executing file
   as program" (or, in a terminal in that folder: `chmod +x Mortalcraft-Launcher-Linux`).
4. Start it (double-click it, or `./Mortalcraft-Launcher-Linux` in a terminal). From then on it is in your
   applications menu as Mortalcraft.

If you run Wine some other way (a Flatpak Wine, your own Wine prefix), say so on the launcher's Settings page. The
launcher writes what it did to `~/.config/Mortalcraft/launcher.log`. It needs a system from 2022 or newer (Ubuntu
22.04, Fedora 36, Debian 12 or later).

## Good to know

- This is a test server. It can restart at any moment, and things change often.
- A Quartermaster stands at every starting spot and in the capitals. It gives out skill books, gear and ready-made
  character set-ups for free, so you can try anything without earning it first.
- Found something broken or odd? Type `/mcnote` followed by what happened. It is saved with where you were and
  what you were doing.

## If something doesn't work

- "Can't reach the server": it may be restarting, so try again in a minute. Check the address you typed too.
- "The Wow.exe in that folder isn't the original": the launcher only works with an unchanged 3.3.5a `Wow.exe`.
- Anything else: the launcher writes what it did to `%AppData%\Mortalcraft\launcher.log`. Send that file to
  whoever invited you.
  On Linux it is `~/.config/Mortalcraft/launcher.log`.
- The game looks wrong or won't start with the Vulkan renderer (DXVK) on: turn it off on the Settings page.
- The game is slow, looks wrong or won't start with Lumenveil on: turn it off on the Settings page, or press Ctrl+Shift+F
  in the game to see it without. Its own log, `CoAVolFog.log` beside the game, goes into Report a problem.

## Credits

The optional Vulkan renderer is [DXVK](https://github.com/doitsujin/dxvk) by Philip Rebohle and its contributors,
shipped unchanged under its zlib licence (`dxvk-LICENSE.txt` in each release).

The optional fog, light and water are [Lumenveil](https://github.com/lumenveil/Lumenveil), free software under the GPL
2.0 by its own authors. Mortalcraft doesn't hand it out: when you turn it on, the launcher downloads its official
release from Lumenveil's own page and checks it against the hash in Mortalcraft's signed list.
