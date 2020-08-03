Thermal Monitor
---------------
Plasma 5 applet for monitoring CPU, GPU and other available temperature sensors.

Originally from: https://github.com/kotelnik/plasma-applet-thermal-monitor
I have no affiliation with this project, but I'm tired of manually patching this plugin on new installations, so this one has (some) PRs merged.

### Requirement for Fedora

Packages required:
- `kf5-plasma-devel`
- `extra-cmake-modules`

### Requirement for Arch

Packages required for runtime:
- `plasma-workspace`
- `qt5-graphicaleffects`

Packages required for building:
- `extra-cmake-modules`

Alternatively, you can use the [plasma5-applets-thermal-monitor-git](https://aur.archlinux.org/packages/plasma5-applets-thermal-monitor-git/) AUR package.

### INSTALLATION

```sh
$ git clone --depth=1 https://gitlab.com/agurenko/plasma-applet-thermal-monitor.git
$ cd plasma-applet-thermal-monitor/
$ mkdir build
$ cd build
$ cmake .. -DCMAKE_INSTALL_PREFIX=/usr
$ sudo make install
```

### UNINSTALLATION

```sh
$ cd plasma-applet-thermal-monitor/build/
$ sudo make uninstall
```

or

```sh
$ sudo rm -r /usr/share/plasma/plasmoids/org.kde.thermalMonitor
$ sudo rm /usr/share/kservices5/plasma-applet-org.kde.thermalMonitor.desktop
```

### LICENSE

This project is licensed under the [GNU General Public License v2.0](https://www.gnu.org/licenses/gpl-2.0.html) and is therefore Free Software. A copy of the license can be found in the [LICENSE file](LICENSE).
