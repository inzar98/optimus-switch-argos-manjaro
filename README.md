
         # ARGOS DEVELOPMENT IS STOPPED. FOR GNOME 3.32 USE THİS FORK https://github.com/p-e-w/argos/pull/76
         # I can fork it too if anyone want...
         # You can fallow instalition section for Argos 3.32
         # THIS FORK STILL WIP


# Argos Script For Optimus-Switch
Gnome Shell Indicator for Optimus-Switch, using Argos API

Screenshot was first release. Added icon switch for after gpu switching.

![NVidia Prime Argos Indicator](https://github.com/inzar98/optimus-manager-argos/blob/master/screenshots/optimus-manager-1.png)                                       

#### Requirements
- [Argos] Gnome Shell extension. Look for Installition section
- [Optimus-Switch](https://forum.manjaro.org/t/call-for-testing-optimus-switch/) Awesome Optimus Switch script!
- Zenity for dialog window By @ArionWT
- Gksu


#### Installation
Install [Argos](https://extensions.gnome.org/extension/1176/argos/) Gnome-Shell extension.
FOR GNOME 3.32 USE THİS FORK https://github.com/p-e-w/argos/pull/76

```
! [ -d "~/.local/share/gnome-shell/extensions" ] && mkdir --parents ~/.local/share/gnome-shell/extensions || trueg
cd optimus-switch-argos-manjaro
cp argos@pew.worldwidemann.com -r ~/.local/share/gnome-shell/extensions
```
*** Restart Gnome-Shell and activate the extension ***


Create directory `~/.local/share/icons` if it does not exist:
```
! [ -d "~/.local/share/icons" ] && mkdir --parents ~/.local/share/icons || trueg
```

Then:
```
git clone https://github.com/inzar98/optimus-switch-argos-manjaro.git
cd optimus-switch-argos-manjaro

    # copy icons (not necessary)
    cp -v icons/* ~/.local/share/icons/

# copy 'Optimus-Switch' to 'argos' folder
cp -v Optimus-Switch ~/.config/argos/

# Thats All !
```
#### Uninstall
```
# remove icons
rm ~/.local/share/icons-to-delete/{nvidia-active-symbolic.svg,nvidia-inactive-symbolic.svg,prime-indicator-intel.svg,prime-indicator-intel-symbolic.svg,prime-indicator-nvidia.svg}


# remove argos extension script
rm ~/.config/argos/Optimus-Switch



