This dwm 6.4 (712d663, 2023-01-28) is forked from the original dwm repo at [DWM](https://git.suckless.org/dwm).

For a short period of time I had been using [dwm flexipatch](https://github.com/bakkeby/dwm-flexipatch) which was difficult to maintain.

Refer to [https://dwm.suckless.org/](https://dwm.suckless.org/) for details on the dwm window manager, how to install it and how it works.
Browsing patches? There is a [map of patches](https://coggle.it/diagram/X9IiSSM6PTWOM9Wz) diagram which tries to organise patches into categories.


---

### Changelog:

2023-01-30 - Initial Version


### Patches included:


   - [alpha](https://dwm.suckless.org/patches/alpha/)
      - adds transparency for the status bar

   - [autostart](https://dwm.suckless.org/patches/autostart/)
      - makes dwm run `~/.dwm/autostart_blocking.sh` and `~/.dwm/autostart.sh &` on startup

   - [bar_height](https://dwm.suckless.org/patches/bar_height/)
      - allows the bar height to be explicitly set rather than being derived from font

   - [bartabgroups](https://dwm.suckless.org/patches/bartabgroups/)
      - turns the titlebar area into a mfact-respecting tab-bar showing each client's title

   - [dwmblocks](https://gist.github.com/danbyl/54f7c1d57fc6507242a95b71c3d8fdea)
      - signal integration to use dwm with a patched [dwmblocks](https://github.com/torrinfail/dwmblocks)
      - combined with the statuscmd patch this gives a clickable statusbar

   - [hidevacanttags](https://dwm.suckless.org/patches/hide_vacant_tags/)
      - prevents dwm from drawing tags with no clients (i.e. vacant) on the bar

   - [scratchpad](https://dwm.suckless.org/patches/scratchpad/)
      - the scratchpad patch allows you to spawn or restore a floating terminal window

   - [swallow](https://dwm.suckless.org/patches/swallow/)
      - this patch adds "window swallowing" to dwm as known from Plan 9's windowing system rio
      - clients marked with isterminal in config.h swallow a window opened by any child process,
        e.g. running xclock in a terminal
      - closing the xclock window restores the terminal window in the current position

   - [systray](https://dwm.suckless.org/patches/systray/)
      - adds system tray in the status bar

   - [resetnmaster](https://dwm.suckless.org/patches/resetnmaster/)
      - resets # of master windows into one
      
   - [columns](https://dwm.suckless.org/patches/columns/)
      - column layout. make sure you increase the # of masters to this layout to work in an expected manner
      
   - [taggrids](https://dwm.suckless.org/patches/taggrid/)
      - ability to place tags in rows like in many other window managers like xfce ore OpenBox.


### Layouts included:
   This is in addition to the monocle tile and floating that comes along with vanilla dwm.

   - [columns](https://dwm.suckless.org/patches/columns/)
      - same as the default tile layout except clients in the master area are arranged in columns
        (i.e. left to right)
