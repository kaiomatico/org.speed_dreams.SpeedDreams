# Updated Speed Dreams Flatpak
I updated the Flatpak SDK and the dependencies of the Speed Dreams flatpak. Original forked from here: 
- https://github.com/flathub/org.speed_dreams.SpeedDreams
- https://flathub.org/apps/details/org.speed_dreams.SpeedDreams

# Installation instructions
```
flatpak install flathub org.freedesktop.Platform//20.08 org.freedesktop.Sdk//20.08
git clone --recurse-submodules https://github.com/kaiomatico/org.speed_dreams.SpeedDreams.git
cd org.speed_dreams.SpeedDreams
flatpak-builder build-dir org.speed_dreams.SpeedDreams.yaml --force-clean
flatpak-builder --user --install build-dir org.speed_dreams.SpeedDreams.yaml --force-clean
flatpak run org.speed_dreams.SpeedDreams
```
# Control
The default control scheme uses the mouse to steer. If this is not desired adjust the controls in the settings to steer left and right with the arrow keys. To switch the camera outside of the car press `F3`

# Uninstall instructions
```
flatpak uninstall --delete-data org.speed_dreams.SpeedDreams
```

