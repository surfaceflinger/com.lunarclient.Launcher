# [flatpak] com.lunarclient.Launcher

## How to build

1. Clone this repository: `git clone --recurse-submodules https://github.com/Morelcia/com.lunarclient.Launcher.git`
2. Add flathub repository: `flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo`
3. Install Freedesktop SDK with: `flatpak install flathub org.freedesktop.Sdk//20.08`
4. Install Freedesktop Platform with: `flatpak install flathub org.freedesktop.Platform//20.08`
5. Install Electron base with `flatpak install flathub org.electronjs.Electron2.BaseApp/x86_64/20.08`
6. cd into cloned repo: `cd com.lunarclient.Launcher`
7. Build and install package: `flatpak-builder --user --install ./lunar com.lunarclient.Launcher.yml --force-clean`

## How to run

`flatpak run com.lunarclient.Launcher`

or just use .desktop file that should be already detected by your applications menu

## schizo

For max security you could prob swap glfw for wayland one and just use it on wayland or embed weston composer and run it on x11 while not giving lunar access to anything x11 related x
