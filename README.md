# meow

fixed KDE 1 binaries for Arch Linux (or arch-based distros)

it is recommended to install this on Arch Linux without any desktop environments or greeters installed

### how to install
- install qt1 first, both files
- then install kdelibs, both files
- and then just install kdebase, both files as well

**use `pacman -U (file)` to install them**

after all of that is done, make a new .xinitrc file and add this in
```
export PATH=/opt/kde1/bin:$PATH
export LD_LIBRARY_PATH=/opt/qt1/lib:/opt/kde1/lib
exec startkde
```

once you did all of this, type `startx` to start KDE 1

shoutout to [@RandomVee (Cookiaria)](https://github.com/RandomVee?tab=repositories) for testing this out on a VM ! !
