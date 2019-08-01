# Base files for Anonymity Distribution Gateways #

Provides a /usr/share/anon-gw-base-files/gateway marker file, which allows
other packages to identify, that this is an anonymity distribution gateway.

Do not remove, unless you no longer wish to use an anonymity distribution
gateway.
## How to install `anon-gw-base-files` using apt-get ##

1\. Download [Whonix's Signing Key]().

```
wget https://www.whonix.org/patrick.asc
```

Users can [check Whonix Signing Key](https://www.whonix.org/wiki/Whonix_Signing_Key) for better security.

2\. Add Whonix's signing key.

```
sudo apt-key --keyring /etc/apt/trusted.gpg.d/whonix.gpg add ~/patrick.asc
```

3\. Add Whonix's APT repository.

```
echo "deb https://deb.whonix.org buster main contrib non-free" | sudo tee /etc/apt/sources.list.d/whonix.list
```

4\. Update your package lists.

```
sudo apt-get update
```

5\. Install `anon-gw-base-files`.

```
sudo apt-get install anon-gw-base-files
```

## How to Build deb Package ##

Replace `apparmor-profile-torbrowser` with the actual name of this package with `anon-gw-base-files` and see [instructions](https://www.whonix.org/wiki/Dev/Build_Documentation/apparmor-profile-torbrowser).

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Professional Support](https://www.whonix.org/wiki/Professional_Support)

## Donate ##

`anon-gw-base-files` requires [donations](https://www.whonix.org/wiki/Donate) to stay alive!
