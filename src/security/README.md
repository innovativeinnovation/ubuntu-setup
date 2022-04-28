# Security

## Disk Encryption

### Full disk encryption

The Ubuntu 22.04 installer proposes to encrypt your disk for security.

Every time the system starts, you will have to enter the passkey for
the encrypted drive. Without the pass key, Ubuntu won't boot.

## Firewall

The Uncomplicated Firewall (ufw) is a frontend for iptables and is
particularly well-suited for host-based firewalls.

By default, ufw is disabled. You can check the status of your firewall with:

```bash
sudo ufw status
```

To enable the firewall:

```bash
sudo ufw enable
```

To disable the firewall:

```bash
sudo ufw disable
```

To manage the firewall via a graphical user interface:

```bash
sudo apt install gufw
```

## Antivirus

[ClamAV](http://www.clamav.net/) is an open source antivirus engine for
detecting trojans, viruses, malware & other malicious threats.

To install ClamAV:

```bash
sudo apt install clamav
```

To manually update the threat database:

```bash
sudo systemctl stop clamav-freshclam
sudo freshclam
sudo systemctl start clamav-freshclam
```

To scan the `home` directory:

```bash
clamscan --infected --remove --recursive /home
```

To run ClamAV as a Daemon:

```bash
sudo apt install clamav-daemon
```

To install the front-end (GUI) client:

```bash
sudo apt install clamtk
```
