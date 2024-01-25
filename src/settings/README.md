# System Preferences

First thing you should do is update the system.

```bash
sudo apt update
sudo apt upgrade
```

If this is a new computer, there are a couple tweaks you could make to the
Settings. **These settings are all optional, consider them suggestions.**

## Settings

### Appearance

* Auto-hide the Dock -> On
* Icon size -> 32

### Privacy

#### File History & Trash

* File History -> Off

#### Screen Lock

* Automatic Screen Lock -> On
* Show Notifications on Lock Screen -> Off

#### Diagnostics

* Send error reports to Canonical -> Manual

### Power

* Dim screen -> Off
* Battery Percentage -> On

### Region & Language

* Choose the right format

## Software & update

### Additional Drivers

Follow the specific instructions provided on the screen.

## Gnome Tweak Tool

```bash
sudo apt install gnome-tweaks
```

### Fonts

* Ubuntu Mono Regular -> 11px

### Top Bar

* Weekday -> On
* Date -> On
* Seconds -> On
* Week Numbers -> On

## Gnome Shell Extensions

```bash
sudo apt install gnome-shell-extensions gnome-shell-extension-manager
```

Search and open the "Extensions Manager".

Must have:

* OpenWeather - Weather extension to display weather information
* Clipboard Indicator - Clipboard Manager extension
* User Themes - Load shell themes from user directory.
