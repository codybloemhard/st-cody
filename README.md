# st-cody
My Suckless ST fork.
## Extra Features
- Scrollback per page
- Translucent background with custom (correct?) blending(alpha = 0 means no bg colour no matter what the bg colour is set to)
- Alpha ignored in selected text (to support alpha = 0)
- Colours can be set with cli arguments
- Colours can be set with Xresources
- Colours can be refreshed live with `pkill -USR1 '^st$'`
- Disabled Bold == Bright (Bold is Bold and Bright is Bright).
## Patches aplied
- st-alpha-0.8.2.diff
- st-scrollback-20200419-72e3f6c.diff
- st-colors-at-launch-0.8.4.diff
- st-xresources-20200604-9ba7ecf.diff
- st-bold-is-not-bright-20190127-3be4cf1.diff (just quickly by hand)
## Loosly based on
- st-externalpipe-signal-0.8.2.diff
## Bugs
Xresources works normally and with -c flag(to set class), however it does not work with -n flag(set name).
I don't know why but I use -c now instead of -n and changed my i3 config to have live colour refreshable scratchpad.
## Some Shortcuts
### (Meant for QGMLWY layout)
C(Control), S(Shift)
- C-S c = copy
- C-S v = paste
- C i = scroll up a page
- C k = scroll down a page
