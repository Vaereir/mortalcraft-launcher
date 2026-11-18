# Mortalcraft

Mortalcraft is a World of Warcraft 3.3.5a server that is being tested. You can only play if you were invited.

## What you need

- An invitation: an account name, a password and the server's address.
- Your own copy of World of Warcraft 3.3.5a (build 12340, English). Use a separate copy for Mortalcraft, because
  its files change the game.
- [Tailscale](https://tailscale.com/download) (free). Sign in and accept the invitation to the server you were sent.

## Getting started

1. Download `Mortalcraft-Launcher.exe` from the [latest release](../../releases/latest).
2. Put it in your game folder, next to `Wow.exe`, and start it. Windows will say it doesn't know who made it:
   choose "More info", then "Run anyway".
3. Type the server address you were given and press Play.
4. Log in with your account name and password.

Always start the game with the launcher and leave its window open while you play. It keeps your files up to date
and carries your connection to the server.

## Good to know

- This is a test server. It can restart at any moment, and things change often.
- A Quartermaster stands at every starting spot and in the capitals. It gives out skill books, gear and ready-made
  character set-ups for free, so you can try anything without earning it first.
- Found something broken or odd? Type `/mcnote` followed by what happened. It is saved with where you were and
  what you were doing.

## If something doesn't work

- "Can't reach the server": check that Tailscale is running and connected. The server may also be switched off.
- "The Wow.exe in that folder isn't the original": the launcher only works with an unchanged 3.3.5a `Wow.exe`.
- Anything else: the launcher writes what it did to `%AppData%\Mortalcraft\launcher.log`. Send that file to
  whoever invited you.
