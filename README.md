## TUXEDO One
##### A modern flat theme with a combination of light and dark elements. It supports GNOME, Unity, Xfce and Openbox.

## Install It

### Distro Packages
Not available yet.

## Build It

First, you need to compile the theme using the [Sass](http://sass-lang.com/) compiler.

To install Sass, install Ruby and the gem command using your distribution's package manager. Then install `sass` with the `gem` command,

`gem install sass`

You'll also need the ```glib-compile-schemas``` and  ```gdk-pixbuf-pixdata``` commands in your path to generate the gresource binary. Install them using your distribution's package manager.

|Distro|Commands|
|:----:|:----:|
|![arch][arch] &nbsp;![antergos][antergos]|`sudo pacman -S glib2 gdk-pixbuf2`|
|![opensuse][opensuse]|`sudo zipper install glib2-devel gdk-pixbuf-devel`|
|![fedora][fedora]|`sudo dnf install glib2-devel gdk-pixbuf2-devel`|
|![debian][debian] &nbsp;![ubuntu][ubuntu]|`sudo apt-get install libglib2.0-dev libgdk-pixbuf2.0-dev libxml2-utils`|

After installing all the dependencies, change to the cloned directory and, run the following in Terminal,

```sh
sudo make install
```

To set the theme in GNOME, run the following commands in Terminal,

```sh
gsettings set org.gnome.desktop.interface gtk-theme "TUXEDOOne"
gsettings set org.gnome.desktop.wm.preferences theme "TUXEDOOne"
```

To set the theme in Xfce, run the following commands in Terminal,

```sh
xfconf-query -c xsettings -p /Net/ThemeName -s "TUXEDOOne"
xfconf-query -c xfwm4 -p /general/theme -s "TUXEDOOne"
```

### Requirements

GTK+ 3.18 or above

Murrine theme engine

### Code and license

Report bugs or contribute at [GitHub](https://github.com/numixproject/numix-gtk-theme)

License: GPL-3.0+


[antergos]: https://www.dropbox.com/s/tju7maccr328w87/logo-square26x26.png?dl=1 "antergos"
[arch]: https://www.dropbox.com/s/q8ypd345cqcd0b5/archlogo26x26.png?dl=1 "arch"
[fedora]: https://www.dropbox.com/s/b8q448vuwopb0cl/fedora-logo.png?dl=1 "fedora"
[openSUSE]: https://www.dropbox.com/s/jhirpw85ztgl59h/Geeko-button-bling7.png?dl=1 "openSUSE"
[ubuntu]: https://www.dropbox.com/s/nev98nld2u1qbgl/ubuntu_orange_hex.png?dl=1 "ubuntu"
[debian]: https://www.dropbox.com/s/jg7pypm1zk9qjt6/openlogo-nd-25.png?dl=1 "debian"

