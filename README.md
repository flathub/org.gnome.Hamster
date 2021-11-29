
# Flatpak package for Hamster Time Tracker

This repo contain the build file for Hamster 
based on the original work in the upstream repo.

* https://flathub.org/apps/details/org.gnome.Hamster
## Installation

If you downloaded the file with the Hamster bundle (ending in .flatpak), you can directly install it with:

    flatpak install --reinstall Hamster.flatpak

If you would like to install Hamster only for your user, please pass the `--user` option to the above command.

After installation, if you need to invoke Hamster from the command line, you can do so with:

    flatpak run org.gnome.Hamster [args...]

To remove the installed flatpak, just run:

    flatpak uninstall org.gnome.Hamster
## Migration data to Flatpak

If you would like to retain your data from a non-flatpak installation, 
you can do so by running:

```shell
gio copy -b \
    ~/.local/share/hamster/hamster.db \
    ~/.var/app/org.gnome.Hamster/data/hamster/
```

After checking everything works, you can remove the original database.
## Links

* [Hamster project github page](https://github.com/projecthamster/hamster)
* [Hamster on FlatHub](https://flathub.org/apps/details/org.gnome.Hamster)
