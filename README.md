# F1 Live Timing - GNOME Extension

Show Formula 1 session or race times directly in the Gnome Shell

## 📌 Features
- Live Formula 1 session and race timings
- Integration with the OpenF1 API
- Dynamic icon in the top bar
- Dropdown menu with real-time updated times
- API key configuration support

## 🛠️ Installation

### 1. Install from GNOME Extensions Website (Recommended)
Once published, you can install the extension directly from the [GNOME Extensions website](https://extensions.gnome.org/). After installation, enable it via GNOME Extensions or GNOME Tweaks.

### 2. Manual Installation (For Development)
If you are developing or modifying the extension, you can manually install it with the following steps:

#### Requirements
Make sure you have the necessary packages installed on Fedora:
```bash
sudo dnf install gnome-shell-extension-tool gnome-shell-devel gjs libgee
```

#### Clone the repository into the GNOME extensions folder:
```bash
git clone https://github.com/DerefDev/f1-live-timing.git ~/.local/share/gnome-shell/extensions/f1-live-timing@deref.dev.gmail.com
```

Compile the settings schemas:
```bash
glib-compile-schemas ~/.local/share/gnome-shell/extensions/f1-live-timing@deref.dev.gmail.com/schemas/
```

Enable the extension:
```bash
gnome-extensions enable f1-live-timing@deref.dev.gmail.com
```

#### Restart GNOME Shell
If the extension does not appear, try restarting GNOME Shell:
- **Xorg**: Press `Alt + F2`, type `r`, and press `Enter`.
- **Wayland**: Log out and log back in.

## 🔑 API Key Configuration

1. Open the extension settings.
2. Enter your OpenF1 API key.
3. Save and restart the extension.

## 🔄 Uninstallation

If installed via the GNOME Extensions website, you can remove it from the GNOME Extensions app.

For manual installations:
```bash
rm -rf ~/.local/share/gnome-shell/extensions/f1-live-timing@deref.dev.gmail.com
```

## 📜 License
This project is licensed under the **GPLv3 License**. See the [LICENSE](LICENSE) file for more details. Contributions, issues, and pull requests are welcome!

## 🏎️ Author
Developed by [DerefDev](https://github.com/DerefDev). If you have suggestions or issues, feel free to open an issue in the repository.
