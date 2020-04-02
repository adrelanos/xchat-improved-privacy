# Improves XChat Privacy Settings #

As per https://trac.torproject.org/projects/tor/wiki/doc/TorifyHOWTO/XChat.

Moves the following files:
- /usr/lib/xchat/plugins/python.so
- /usr/lib/xchat/plugins/tcl.so
- /usr/lib/xchat/plugins/perl.so
to /usr/share/xchat-improved-privacy, so these plugins get disabled by
default.
## How to install `xchat-improved-privacy` using apt-get ##

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

5\. Install `xchat-improved-privacy`.

```
sudo apt-get install xchat-improved-privacy
```

## How to Build deb Package from Source Code ##

Can be build using standard Debian package build tools such as:

```
dpkg-buildpackage -b
```

See [instructions](https://www.whonix.org/wiki/Dev/Build_Documentation/xchat-improved-privacy). (Replace `package-name` with the actual name of this package.)

## Contact ##

* [Free Forum Support](https://forums.whonix.org)
* [Professional Support](https://www.whonix.org/wiki/Professional_Support)

## Donate ##

`xchat-improved-privacy` requires [donations](https://www.whonix.org/wiki/Donate) to stay alive!
