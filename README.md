# druid

a super-basic terminal for crow

...and some pythong utils

## setup

run `make`

then run `./druid`

`q` to quit

## port

default connects to

```
/dev/ttyAMA0
```

specify an arg for different port ie

```
./druid /dev/ttyAMA1
```

## BROKEN

- DOESN'T WORK ON MACOS. serial port open just hangs.
- sloppy use of `getch()` means chars aren't reported until CR, so there are double-prints etc
- crow prints will interrupt command typing
- no readline niceties (up-arrow)

## TODO

- hack into old command-line maiden, use readline and ncurses etc


---

## python utils

- requires pyserial. install using `pip install pyserial`

```
python upload.py test-2.lua
```

tested only on linux (assumes `/dev/ttyACM0`)
