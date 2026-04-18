# hypr-res-picker
Resolution picker for the hyprland WM written in bash.

### Usage
You can execute hypr-res-picker from a terminal, or preferrably bind it to a key

`bash
hypr-res-picker "auto, 1, vrr, 1" "dmenu"
`

`
bind = $mainMod SHIFT, P, exec, hypr-res-picker "auto, 2" "wofi -d"
`
hypr-res-picker needs a dmenu application for the gui, you can use whatever you want as long as it has a dmenu mode

You can specify your preferred command as the second arguement, as shown above at the hyprland config

If there is no second arguement, hypr-res-picker defaults to dmenu


First arguement will be the options passed to hyprctl

Defaults to "auto, 1"

### Installation
hypr-res-picker expects all of the scripts to be in the path. The stock installation script just copies the scripts into /usr/local/bin/ .
Of course this makes it so that you have to run the install script as sudo. There is not much to do for an installation, so you can do it manually as well.
`bash
sudo ./install
`
