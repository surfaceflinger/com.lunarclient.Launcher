# [flatpak] com.lunarclient.Launcher

## How to build

1. Clone this repository: `git clone --recurse-submodules https://github.com/Morelcia/com.lunarclient.Launcher.git`
2. Add flathub repository: `flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo`
3. cd into cloned repo: `cd com.lunarclient.Launcher`
4. Build and install package: `flatpak-builder --user --install-deps-from=flathub --install ./lunar com.lunarclient.Launcher.yml --force-clean`

## How to run

`flatpak run com.lunarclient.Launcher`

or just use .desktop file that should be already detected by your applications menu

## schizo

For max security you could prob swap glfw for wayland one and just use it on wayland or embed weston composer and run it on x11 while not giving lunar access to anything x11 related x

## Alternatives
- macOS: [makindotcc/sandboxexec_LunarClient](https://github.com/makindotcc/sandboxexec_LunarClient)

![Screenshot](https://nekopon.pl/syf/lunarsandbox.png)
