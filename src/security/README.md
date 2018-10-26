# Security

### Disk Encryption

###### Full disk encryption

The Ubuntu 18.04 installer proposes to encrypt your disk for security. Choosing the
LVM option is optional but recommended.

Every time the system starts, you will have to enter the passkey for
the encrypted drive. Without the pass key, Ubuntu won't boot.

###### Encrypt The Home Folder

Ubuntu 18.04 doesn't include an option in the installer to encrypt the `home`
directory. This option was removed from the Ubuntu installer because it
uses eCryptfs, which is considered "buggy, under-maintained", and the
recommended alternative is a full disk encryption using LUKS.

If you still want to encrypt your `home` folder, follow these steps.

```bash
sudo apt install ecryptfs-utils cryptsetup
sudo adduser foobar
sudo usermod -aG sudo foobar
```

Logout and login as foobar. Then:

```bash
sudo ecryptfs-migrate-home -u <user>
```

where `<user>` is your primary account. Logout from foobar and login as
`<user>` (do not reboot!).

Run:

```bash
ecryptfs-unwrap-passphrase
```

and save this somewhere safe! Reboot and if everything is ok, you can
safely remove the temporary user foobar as well as the backup.

```bash
sudo deluser --remove-home foobar
ls /home
```

and remove the folder `<user>.xxxxxxxx`.

### Firewall

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

### Antivirus

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
