# My collection of xbps packages/templates
This small project contains some packages that mainstream Void Linux repositories either don't provide or refuse to include

> NOTE: I don't provide prebuilt musl packages, and not every template here builds with musl.

Currently added packages

| Package                 | Version             |
| ----------------------- | ------------------- |
| darkly                  | 0.5.22              |
| rofi-wayland            | 1.7.9+wayland1      |
| vesktop                 | 1.5.8               |
| ttf-jetbrains-mono-nerd | 3.4.0               |
| proton-vpn-gtk-app      | 4.9.7               |


# Installation 
You can add this repository by creating a file at `/etc/xbps.d/10-extra-pkgs.conf` with following text:
```
repository=https://raw.githubusercontent.com/VanillaDaFur/xbps-extra/repository-x86_64-glibc
```

To do this quickly, you can run:
```
echo 'repository=https://raw.githubusercontent.com/VanillaDaFur/xbps-extra/repository-x86_64-glibc' | sudo tee /etc/xbps.d/10-extra-pkgs.conf
```

Then refresh your repositories.
```
sudo xbps-install -S
```
That's it! You can now install packages from this repository.
> NOTE: Again, this repository *ONLY* provides glibc binaries; musl binaries are not available.

# Credits
- **[hyprland-void](https://github.com/Makrennel/hyprland-void)** for his nice build scripts
