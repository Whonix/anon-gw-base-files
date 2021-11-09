# Base files for Anonymity Distribution Gateways #

Provides a /usr/share/anon-gw-base-files/gateway marker file, which allows
other packages to identify, that this is an anonymity distribution gateway.

Whonix-Gateway grub branding, motd and issue banner.

Sets Xfce desktop and display setting, wallpaper and desktop icons.
/etc/skel/.config/xfce4/xfconf/xfce-perchannel-xml/xfce4-desktop.xml.anondist

Do not remove, unless you no longer wish to use an anonymity distribution
gateway.
## How to install `anon-gw-base-files` using apt-get ##

1\. Download the APT Signing Key.

```
wget https://www.whonix.org/derivative.asc
```

Users can [check Whonix Signing Key](https://www.whonix.org/wiki/Whonix_Signing_Key) for better security.

2\. Add the APT Signing Key..

```
sudo cp ~/derivative.asc /usr/share/keyrings/derivative.asc
```

3\. Add the derivative repository.

```
echo "deb [signed-by=/usr/share/keyrings/derivative.asc] https://deb.whonix.org bullseye main contrib non-free" | sudo tee /etc/apt/sources.list.d/derivative.list
```

4\. Update your package lists.

```
sudo apt-get update
```

5\. Install `anon-gw-base-files`.

```
sudo apt-get install anon-gw-base-files
```

## How to Build deb Package from Source Code ##

Can be build using standard Debian package build tools such as:

```
dpkg-buildpackage -b
```

See instructions. (Replace `generic-package` with the actual name of this package `anon-gw-base-files`.)

* **A)** [easy](https://www.whonix.org/wiki/Dev/Build_Documentation/generic-package/easy), _OR_
* **B)** [including verifying software signatures](https://www.whonix.org/wiki/Dev/Build_Documentation/generic-package)

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Professional Support](https://www.whonix.org/wiki/Professional_Support)

## Donate ##

`anon-gw-base-files` requires [donations](https://www.whonix.org/wiki/Donate) to stay alive!
