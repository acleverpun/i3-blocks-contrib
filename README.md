Example config:

```
# defaults
separator_block_width=16
command=$HOME/.config/i3/blocks/$BLOCK_NAME


[mediaplayer]
color=#00ffaf
interval=2
signal=11


[weather]
align=right
color=#ff5f00
interval=1800


[keyboard]
interval=1
label=
signal=10


[yaourt]
interval=7200
label=
signal=10


[cpu]
align=center
color=#ffff00
interval=3
label=
min_width="100%"


[memory]
align=center
color=#00ffaf
interval=3
label=
min_width="100%"


[disk-root]
command=$HOME/.config/i3/blocks/disk-free
instance=/
interval=60
separator=false


[disk-data]
command=$HOME/.config/i3/blocks/disk-free
instance=/media/data
interval=60


[download]
align=right
color=#00afff
command=$HOME/.config/i3/blocks/bandwidth rx
interval=1 # IMPORTANT
label=
min_width="000 kB/s"


[upload]
align=right
color=#ff5f5f
command=$HOME/.config/i3/blocks/bandwidth tx
interval=1 # IMPORTANT
label=
min_width="000 kB/s"


[ethernet]
color=#875fd7
command=$HOME/.config/i3/blocks/network
instance=enp*
interval=once
label=


[wireless]
color=#5f00af
command=$HOME/.config/i3/blocks/network
instance=wlp*
interval=once
label=


[battery]
color=#66ff33
interval=30


[sound]
align=right
color=#ffff00
instance=Master
interval=once
signal=11


[date]
interval=3600
label=
min_width=0000-00-00


[time]
label=
min_width=00:00:00
interval=1
```
