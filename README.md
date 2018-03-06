# Breeze2000
Breeze2000 is a fork of KDE Breeze decoration that aims to look like Windows 2000 with the gradients while preserving the main look of Breeze.

![Screenshot](https://github.com/alex47/Breeze2000/blob/master/Breeze2000_Screenshot3.png)

The following description is mainly copied from [SierraBreeze](https://github.com/ishovkun/SierraBreeze).


## Dependencies
There are some dependencies you'll need to install. Some people suggested using the following commands:
### Ubuntu
``` shell
sudo apt install libkf5config-dev libkdecorations2-dev libqt5x11extras5-dev qtdeclarative5-dev extra-cmake-modules libkf5guiaddons-dev libkf5configwidgets-dev libkf5windowsystem-dev libkf5coreaddons-dev
```

### Arch Linux
``` shell
sudo pacman -S kdecoration qt5-declarative qt5-x11extras    # Decoration
sudo pacman -S cmake extra-cmake-modules                    # Installation
```

## Installation
In order to install the theme and add it to your decorations do the following:
``` shell
git clone https://github.com/alex47/Breeze2000
cd Breeze2000
mkdir build
cd build
cmake .. -DCMAKE_INSTALL_PREFIX=/usr -DCMAKE_BUILD_TYPE=Release -DKDE_INSTALL_LIBDIR=lib -DBUILD_TESTING=OFF -DKDE_INSTALL_USE_QT_SYS_PATHS=ON
sudo make install
```
To avoid logging out, issue
``` shell
kwin_x11 --replace &
```
That is it! Your new decoration theme should appear in
*Settings &rarr; Application Style &rarr; Window Decorations*.

## Acknowledgments:
- The authors of Breeze window decorations Martin Gräßlin and Hugo Pereira Da Costa
