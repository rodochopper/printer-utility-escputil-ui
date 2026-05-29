<img width="1140" height="1176" alt="PUEUI" src="https://github.com/user-attachments/assets/0ac18cb6-03a8-4f8a-aaa7-e12879d07446" />
# Printer Utility - Escputil UI

A modern graphical frontend for `escputil` on Linux, designed for both local USB and remote SSH printer maintenance workflows.

![Python](https://img.shields.io/badge/Python-3-blue)
![PyQt6](https://img.shields.io/badge/UI-PyQt6-green)
![Linux](https://img.shields.io/badge/Platform-Linux-orange)
![License](https://img.shields.io/badge/Status-Active-success)

---

## Features

### Printer Maintenance

* Nozzle checks
* Injector cleaning
* Head alignment
* Printer identification
* Printer status information
* Real ink information (if supported by the printer)

### Connection Modes

* Local USB support
* Remote SSH printer maintenance
* Automatic printer device detection

### Ink Management

* Real ink information when available
* Manual estimated ink tracking system
* Adjustable ink levels
* Persistent ink estimation storage

### Desktop Integration

* Native KDE / GNOME support
* Proper Wayland icon integration
* Desktop launcher support
* `.deb` package support

### User Experience

* English and Spanish support
* Saved connection history
* Modern PyQt6 interface
* Clean Linux desktop integration

---

# Screenshots



---

# Installation

## Debian / Ubuntu

Install dependencies:

```bash
sudo apt install escputil printer-driver-escpr python3-pyqt6 python3-paramiko openssh-client
```

Install the `.deb` package:

```bash
sudo apt install ./printer-utility-escputil-ui_0.1.0_all.deb
```

---

# Usage

## Local USB Mode

1. Connect the printer directly to your Linux machine.
2. Open the application.
3. Select **Local USB** mode.
4. Detect or enter the printer device manually.
5. Run maintenance tools.

Example device:

```text
/dev/usb/lp0
```

---

## Remote SSH Mode

1. Enable SSH on the remote Linux machine.
2. Connect the printer to that machine.
3. Enter:

   * IP / Host
   * SSH username
   * SSH password (optional)
4. Detect printer device automatically or enter manually.
5. Run maintenance remotely.

---

# Notes About Ink Levels

Real ink information depends on printer compatibility.

Some printers expose native ink information directly to `escputil`, while others do not.

For unsupported printers, the application includes a manual estimated ink tracking system.

---

# Technologies Used

* Python 3
* PyQt6
* Paramiko
* escputil
* SSH
* Linux desktop integration

---

# Roadmap

* Flatpak support
* AppImage support
* Automatic dependency checking
* Multi-printer profiles
* Dark mode improvements
* Better real ink parsing
* Additional printer compatibility

---

# Project Links

## GitHub

https://github.com/rodochopper

## Support the Project

PayPal:
https://paypal.me/rodochopper

Patreon:
https://www.patreon.com/c/rodochopper

---

# License

This project is currently released as open source software.

License selection pending.

---

# Author

Created by **rodochopper**

Version: **0.1.0**
