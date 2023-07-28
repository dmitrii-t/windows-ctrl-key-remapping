# Windows Ctrl Keys Remapping
Control keys remapping for Windows to move `Left Ctrl` key next to the `Space` key for convenience.

This sets `Scancode Map` key in the registry with the following value

```hexdump
00,00,00,00, # Header: Version. Set to all zeroes
00,00,00,00, # Header: Flags. Set to all zeroes
04,00,00,00, # 4 entries in the map below
1d,00,38,00, # 1st Left Ctrl -> Left Alt
38,00,5b,e0, # 2nd Left Alt -> Left Win
5b,e0,1d,00, # 3rd Left Win -> Left Ctrl
00,00,00,00  # 4th Null entry
```

Other control key codes

```hexdump
1d 00    # Left Ctrl
1d e0    # Right Ctrl
38 00    # Left Alt
38 e0    # Right Alt
5b e0    # Left Windows Key
5c e0    # Right Windows Key
5d e0    # Windows Menu Key
```

[Reference](https://superuser.com/a/1202601/270174)
