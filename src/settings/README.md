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

### Region & Language

* Choose the right format

## Software & update

### Other Software

In order to get access to all the good​ stuff you will need to enable the
Canonical Partners repositories.

### Additional Drivers

Follow the specific instructions provided on the screen.

## Gnome Tweak Tool

```bash
sudo apt install gnome-tweak-tool
```

### Extensions

* Desktop icons -> Off

### Fonts

* Monospace -> 11px

### Top Bar

* Battery Percentage -> On
* Weekday -> On
* Date -> On
* Seconds -> On
* Week Numbers -> On

## Gnome Shell Extensions

```bash
sudo apt install chrome-gnome-shell
```

Go to [https://extensions.gnome.org/](https://extensions.gnome.org/) and
install the browser extension. You can now install any Gnome Shell Extension
by turning on the switch on the web.

Gnome Tweak Tool has a page for managing installed Gnome Shell Extensions.

Must have:

* OpenWeather - Weather extension to display weather information
* Clipboard Indicator - Clipboard Manager extension
* User Themes - Load shell themes from user directory.
