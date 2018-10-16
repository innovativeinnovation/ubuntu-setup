# SSH

[SSH](https://www.ssh.com/), or Secure Shell, is a protocol used to securely
log onto remote systems. It is the most common way to access remote Linux
and Unix-like servers.

### Installation

The client software is part of the default Ubuntu installation.

### Generating a new SSH key

Check for existing SSH keys:

```bash
ls -al ~/.ssh
```

Generate a new SSH key:

```bash
ssh-keygen -t rsa -b 4096 -C "you@example.com"
```

Add your SSH key to the ssh-agent:

```bash
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa
```

### Permissions

If you copied your keys from another computer, permissions should be like
this:

```bash
chmod 700 ~/.ssh
chmod 644 ~/.ssh/authorized_keys
chmod 644 ~/.ssh/known_hosts
chmod 644 ~/.ssh/config
chmod 600 ~/.ssh/id_rsa
chmod 644 ~/.ssh/id_rsa.pub
```

### SSH Config File

You probably log in and out of a half dozen remote servers on a daily basis.
You can add a config file `~/.ssh/config` to simplify your life. For example:

```
Host dev
    HostName dev.example.com
    Port 22000
    User william
```

And then, just:

```bash
ssh dev
```
