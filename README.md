`passwmenu` is a [wofi][]-based interface to [pass][], the standard Unix
password manager.

The design allows you to quickly copy a password to the
clipboard without having to open up a terminal window if you don't already have
one open. If `--type` is specified, the password is typed using [ydotool][]
instead of copied to the clipboard.

The differences to `passmenu` are:
- It's designed wayland rather the Xorg.
- It uses [gopass][] to get passwords without failures.
- Instead of `dmenu` it uses [wofi][].

# Usage

    passwmenu [--type] [wofi arguments...]

[gopass]: https://github.com/gopasspw/gopass
[pass]: http://www.zx2c4.com/projects/password-store/
[wofi]: https://hg.sr.ht/~scoopta/wofi
[ydotool]: https://github.com/ReimuNotMoe/ydotool
