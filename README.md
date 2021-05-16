# i3-named-space-script
Add i3-nws to /usr/local/bin or to your bashrc

It requires jq so make sure you have that installed first\
`sudo apt-get install jq`

Then add the keybind to call it from i3 config

`bindsym $mod+m exec --no-startup-id i3-nws switch`

`bindsym $mod+Shift+m exec --no-startup-id i3-nws move`

The script opens dmenu and grabs the input to be used for the options

`switch` will switch your current workspace to a workspace titled by the input typed into dmenu. Functions just like mod4+number

`move` will move the currently focused container to a workspace titled by the input typed into dmenu. Functions like mod4+shift+number
