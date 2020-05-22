# i3-named-space-script
add i3-nws to /usr/local/bin or wherever

then add the keybind to call it from i3 config

requires jq

ie

`bindsym $mod+m exec --no-startup-id i3-nws switch`

`bindsym $mod+Shift+m exec --no-startup-id i3-nws move`

script opens dmenu and grabs the input to be used for the options

switch will switch your current workspace to a workspace titled by the input typed into dmenu. functions just like mod4+number

move will move the currently focused container to a workspace titled by the input typed into dmenu. functions like mod4+shift+number
