# System Preferences

First thing you should do is update the system.

```bash
sudo apt update
sudo apt upgrade
```

If this is a new computer, there are a couple tweaks you could make to the
Settings. **These settings are all optional, consider them suggestions.**

## Settings

### Dock

* Enable Auto-hide the Dock
* Change icon size to 32

### Region & Language

* Choose the right format

### Privacy

* Screen Lock -> On
* Usage & History -> Off
* Problem Reporting -> Manual

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

### Desktop

* Show icons -> Off
  
### Fonts

* Monospace -> 11px

### Top Bar

* Battery Percentage -> On
* Date -> On
* Seconds -> On

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
* Media Player Indicator - Control MPRIS Version 2 Capable Media Players
* Clipboard Indicator - Clipboard Manager extension
* User Themes - Load shell themes from user directory.
